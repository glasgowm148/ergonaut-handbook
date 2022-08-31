---
title: Panoramica di SigmaUSD
description: 
published: true
date: 2022-08-31T15:01:58.503Z
tags: 
editor: markdown
dateCreated: 2022-08-31T15:01:32.804Z
---






# Panoramica 
IOHK, Ergo ed Emurgo hanno progettato il modello economico di SigmaUSD. Il suo modello economico mantiene le impostazioni conservative per le riserve collaterali ed evita la necessità di liquidazioni. Insieme a ciò, supporta una configurazione di emissione di stablecoin completamente decentralizzata. Pertanto, SigmaUSD offrirà al mondo una stablecoin stabile, semplice e decentralizzata.

I fornitori di riserve inviano Ergs alle riserve della dApp e così facendo coniano ReserveCoins (SigmaRSV). Ciascun SigmaRSV rappresenta una quota delle sottostanti riserve Erg detenute.

Gli utenti SigmaUSD inviano anche Ergs alle riserve dApp; tuttavia, nel loro caso, coniano invece SigmaUSD. Ciò è consentito dal protocollo solo se ci sono riserve sufficienti all'interno della dApp (le riserve sono superiori al coefficiente di riserva minima). In qualsiasi momento, un utente SigmaUSD può riscattare il proprio SigmaUSD in cambio di un importo di Ergs dalle riserve pari al tasso di cambio corrente come fornito dall'oracle pool Erg-USD.

I fornitori di riserve possono riscattare i loro ReserveCoin per Ergs solo se il prezzo di Ergs aumenta (o viene raccolta una quantità sostanziale di commissioni di protocollo) e quindi coprono il valore di tutti i SigmaUSD coniati esistenti più un margine aggiuntivo. Riscattando i loro ReserveCoin, traggono profitto poiché ricevono più criptovaluta di riserva sottostante rispetto a quando hanno coniato i loro ReserveCoin (l'importo maggiore proveniente dagli utenti che hanno coniato SigmaUSD).

> I provider di riserva consentono agli utenti SigmaUSD di godere della stabilità del valore. Da parte loro, i Reserve Provider assorbono il potenziale rialzo (se il valore delle riserve sale tramite il prezzo degli Ergs in aumento rispetto all'USD) e assorbono il potenziale rialzo (se la criptovaluta sottostante in riserva scende di prezzo).
{.is-info}

### Soglia di riserva ERG
- SigmaRSV è un'opzione call su una % di ERG detenuta nella parte di riserva del contratto 

- Le tasse sono continuamente aggiunte agli ERG trattenuti nella riserva man mano che gli utenti interagiscono con il contratto. Questo meccanismo garantisce liquidità e offre un meccanismo di ritorno oltre il trading. SigmaRSV rappresenta un price/book (P/B Ratio) sull'ERG detenuto a riserva.

> È importante comprendere tre meccanismi che influenzano il risultato di ciascun utente di SigmaRSV
{.is-info}

1. Le commissioni si accumulano man mano che gli utenti interagiscono con il contratto. Niente è gratuito.
2. La quota di ERG trattenuta a riserva fluttua (su/giù) man mano che gli utenti interagiscono con il contratto.
3. Il prezzo ERG/USD fluttua (su/giù) mentre gli utenti fanno trading con ERG.

### Panoramica

- Immagina che l'importo della Riserva sia 100 ERG.
- Alice detiene SigmaRSV che rappresenta il 10% del (P/B Ratio) contenuto nelle riserve.
- La posizione SigmaRSV di Alice è un'opzione call su 10 ERG (meno la commissione di cambio)
- Immaginiamo che il prezzo di ERG sia di 2$.
- SigmaRSV di Alice rappresenta 20 $ in ERG (meno la commissione di cambio)

**IL SALDO IN RISERVA PUO' SALIRE**

- Immaginate, in base all'utilizzo, che la riserva ora contenga 114 ERG.
- Alice ha SigmaRSV che rappresenta il 10% del (P/B Ratio) contenuto nelle riserve.
- Il SigmaRSV di Alice rappresenta un'opzione call su 11.4 ERG.
- Immaginiamo che il prezzo di ERG sia ancora 2$.
- Alice ha 22,80$ in ERG (meno la commissione di cambio)

**IL SALDO IN RISERVA PUO' SCENDERE**

- Immagina che, in base all'utilizzo, la riserva ora contenga 90 ERG.
- Alice ha SigmaRSV che rappresenta il 10% del (P/B Ratio) contenuto nelle riserve.
- Il SigmaRSV di Alice rappresenta un'opzione call su 9 ERG.
- Immaginiamo che il prezzo di ERG sia ancora 2$.
- Alice ha 18.00$ in ERG (meno la commissione di cambio)

**IL VALORE, ERG/USD, PUO' SALIRE**

- Immaginate, in base all'utilizzo, che la riserva ora contenga 114 ERG.
- Alice ha SigmaRSV che rappresenta il 10% del (P/B Ratio) contenuto nelle riserve.
- Il SigmaRSV di Alice rappresenta un'opzione call su 11.4 ERG.
- Immaginiamo che il prezzo di ERG sia ancora ORA 3$.
- Alice ha un'opzione call 34,20$ in ERG (meno la commissione di cambio)

**IL VALORE, ERG/USD, PUÒ SCENDERE**

- Immaginate, in base all'utilizzo, che la riserva ora contenga 114 ERG.
- Alice ha SigmaRSV che rappresenta il 10% del (P/B Ratio) contenuto nelle riserve.
- Il SigmaRSV di Alice rappresenta un'opzione call su 11.4 ERG.
- Immaginiamo che il prezzo di ERG sia ancora ORA 1$.
- Alice ha un'opzione call 11.40$ in ERG (meno la commissione di cambio)

# SigmaUSD (Stablecoin) Semplificato

> SigmaUSD rappresenta un'opzione call sul valore in dollari di ERG detenuto in riserva.
{.is-success}

SigmaUSD utilizza l'infrastruttura Oracle Pool di Ergo per calcolare e regolare l'attuale tasso di cambio ERG/USD. La riserva sostiene sempre sigma USD. Il prezzo ERG/USD fluttua (su/giù) mentre gli utenti fanno trading con ERG.

**PANORAMICA DI BASE**

- Bobs ha 20 SigmaUSD che rappresenta un valore di 20 USD in ERG.
- Questi ERG sono tenuti in Riserva.
- Questi 20$ di valore sono garantiti da riserve di almeno
(4x1)(80$ di ERG)(40 ERG @ $2)
- Bob a 2$ Bob può riscattare i suoi 20 SigmaUSD per 10 ERG (meno la commissione di cambio)

**CADUTA DEL VALORE ERG/USD**

- Immaginiamo che il prezzo di ERG scenda da $ 2 a $ 1.
- I 20$ di Bob di valore sono supportati da almeno
(4x1)(80$ di ERG)(80 ERG @ $1)
- Bob può chiamare 20 ERG (meno la commissione di cambio)

**AUMENTA IL VALORE ERG/USD**

- Immaginiamo che il prezzo di ERG aumenti da $ 2 a $ 4.
- I $ 20 di di valore è supportato da almeno
(4x1)(80$ di ERG)(20 ERG @ $4)
- Bob può chiamare 5 ERG (meno la commissione di cambio)

# Quadro a lungo termine di SigmaUSD.

- SigmaUSD è un elemento essenziale per un sistema DeFi funzionante.
- L'attenzione per ERG ora si sposta sulla costruzione delle basi che si è posta.
- Gateway, Dex's, Liquidity Pool, sistemi LETS. È tempo di costruire uso e utilità.
- L'importanza e il significato del valore stabile non possono essere sopravvalutati.
- Questo è fondamentale per la prosperità a lungo termine della rete Ergo ed è importante comprenderlo.

## Incentivi minerari

> SigmaUSD offre ai minatori un modo unico per creare l'infrastruttura di base per un solido sistema DEFI.
{.is-info}

I minatori che gestiscono la rete sono la linfa vitale di un robusto sistema PoW. Un sistema decentralizzato avrà una varietà di attori che consentiranno al sistema di crescere. È essenziale considerare gli incentivi adeguati per soddisfare i bisogni della comunità. Ergo è costruito su solide basi tecnologiche; il mercato finanziario decentralizzato è realizzato tenendo conto delle basi storiche.

Tradizionalmente le banche centrali detenevano l'oro come riserve che sostenevano la valuta. La valuta è stata utilizzata come mezzo di scambio stabile in tutte le economie. Quando stabile o supportato da attività, questo sistema bancario consentiva il commercio e la crescita.

Ci siamo allontanati da un sistema in cui la valuta è supportata da qualsiasi cosa. La valuta di riserva globale viene eseguita su un sistema bancario con requisiti di riserva dello 0%.

I governi di tutto il mondo stanno alimentando continuamente liquidità nell'economia globale. Le banche centrali di tutto il mondo stanno creando denaro e debito a tassi senza precedenti. Questo debito grava su innumerevoli generazioni future, oppure i debiti raggiungeranno un punto di default e ristrutturazione.

Gli asset digitali sono un'alternativa di mercato alla pressione inflazionistica della valuta fiat. La "legge" contenuta nel codice crea scarsità con un programma di emissioni prevedibile. La risorsa in Ergo è ERG. I minatori consumano elettricità e creano questa risorsa elettronica sicura.

Nell'economia globale, l'oro è prodotto dai minatori e venduto a una varietà di attori. Alcuni minatori d'oro possono vendere minerale/prodotto raffinato per aprire mercati, creare contratti OTC o vendere alla banca centrale per tenerlo in riserva.

Ergo ha già percorsi per il mercato aperto tramite gli scambi. OTC, dark pool e un DEX sono in fase di sviluppo per le vendite P2P private. SigmaUSD rappresenta una terza opzione che consente ai minatori l'accesso alla liquidità, la capacità di interagire con un contratto centrale o una banca aggirando il mercato aperto.

L'economia del mining di criptovalute è simile all'economia del trading. Alcuni minatori costruiscono posizioni lunghe. Sono orientati al progetto. Devono trovare un progetto in cui credono e fornire infrastrutture di rete critiche, manutenzione e sviluppo.

Altri minatori agiscono come liberi professionisti; forniscono servizi critici a progetti redditizi. Spesso non accumulano riserve e liquidano continuamente sul mercato aperto per coprire i costi di produzione.

## Punti chiave

- SigmaRSV può offrire ai minatori orientati al progetto un modo per massimizzare le loro posizioni accumulando commissioni. 
Questa classe di minatori può naturalmente trarre vantaggio da SigmaRSV.
- SigmaUSD può offrire liquidità ai minatori freelance per coprire le loro spese in modo decentralizzato, senza scambi. Questa classe di minatori può naturalmente trarre vantaggio da SigmaUSD.
- SigmaUSD offre un incentivo in qualche modo nascosto ai minatori per creare una maggiore stabilità dei prezzi nella risorsa che stanno aiutando a creare e mantenere. Nel tempo, ciò si basa sulla solidità e resilienza della rete.
- Il sistema PoW beneficia della stabilità dei prezzi. I principali fornitori di infrastrutture (miner) operano secondo un modello di ritorno sull'energia investita. Il costo base di questa modalità è Equipaggiamento ed Energia.
- La stabilità dei prezzi aiuta i minatori a prevedere costi/ricavi futuri. SigmaUSD può fungere da meccanismo di stabilizzazione dei prezzi poiché i minatori interagiscono con il contratto in base al loro incentivo. Long vs liquidità.
- Interagire con questo protocollo piuttosto che interagire con il mercato aperto è vantaggioso per tutte le parti.
- La premessa di ERGO è sempre stata un sistema PoW in grado di operare come Riserva Digitale di Oro Programmabile.

## Cos'è una stablecoin?

> È un prodotto derivato. Questo derivato intende creare un modo per stabilizzare la volatilità.
{.is-info}

La stabilità dei prezzi è una parte fondamentale della finanza; senza la stabilità dei prezzi, diventa difficile creare modelli di prodotti finanziari a lungo termine. L'investimento si assume dei rischi; un buon affare, sia on-chain che off, richiede modelli e previsioni per stimare la redditività.

Lo spazio crittografico, per sua natura, è altamente volatile. SigmaUSD e SigmaRSV sono meccanismi per creare valore stabile. Il valore stabile è la base per un'economia prospera.

I derivati ​​sono stati creati per ridurre al minimo la volatilità durante il trading in valute estere.

In un'economia globalizzata, lo spostamento del potere d'acquisto di una valuta rispetto a un'altra può essere una forza altamente distruttiva. L'instabilità interrompe il commercio e distrugge i modelli di business.

La stabilità ha un costo. L'instabilità del prezzo viene spesso aggiunta come premio, a volte come premio per il prezzo e altre volte come premio per interessi.

Il costo di SigmaUSD è l'attuale valore in USD di ERG più una commissione del 2,5%.

Questo è un premio basso, 2,5%.

Qual è il tuo tasso di interesse attuale? Qual è il tasso al quale una banca garantirà un'attività che detieni e offrirà un prestito?

Pochissimi hanno accesso a questo premio basso nell'economia globale e la banca potrebbe non offrire liquidità con una riserva minima o nulla.

SigmaUSD consente a chiunque possieda ERG di collateralizzare il proprio ERG e creare valore liquido. Cosa significa questo?

L'obiettivo a lungo termine sarà quello di creare casi d'uso per questa stablecoin che offre un ritorno oltre questa commissione del 2,5%.

##   Perchè?

> Quando Dapps e l'uso/utilità sono in atto e sostituiscono questa commissione del 2,5%, accade la magia.
{.is-info}

Un utente può prendere il proprio ERG, creare SigmaUSD, quindi utilizzarlo per creare un ritorno maggiore del costo della stabilità del 2,5%. La maggior parte dei modelli di business si basa sulla stabilità e sulla previsione di prezzo/rischio piuttosto che sulla speculazione sugli asset.

SigmaUSD non è solo un'opportunità per prendere una posizione corta su ERG. Piuttosto è un modo per utilizzare il valore di riserva per generare rendimento. Poiché la Defi su Ergo offre possibilità aggiuntive, scambi decentralizzati o pool di liquidità, offre opportunità di crescita per questo valore stabile. Nessuna economia può funzionare correttamente con un'elevata volatilità dei prezzi. Un'economia decentralizzata stabile e robusta richiede un meccanismo monetario stabile e robusto. Idealmente, una valuta supportata da un'attività di riserva per garantirne il valore.

Una volta superato il costo della stabilità del 2,5%, la dinamica del SigmaRSV cambierà radicalmente. Gli utenti avranno un incentivo a coniare/riscattare continuamente SigmaUSD. Forse il valore di ERG aumenterà e un utente potrebbe aver perso un po' di apprezzamento del prezzo; tuttavia, se ha superato la soglia del 2,5%, l'utente ha ottenuto un guadagno netto in USD.

L'utilizzo del valore stabile come mezzo per investire e il superamento della soglia del 2,5% genera rendimenti. Questo trasforma una posizione corta in un modo per creare valore dalla stabilità.

**Immagina i seguenti scenari.**

- Un utente sceglie la stabilità per un premio del 2,5%.
- Anche se il prezzo di ERG si apprezza e l'utente ha la capacità di recuperare. È vero, avranno ERG meno riscattabili, ma la crescita è crescita. Finiscono con una posizione più ampia in USD.
- Forse il valore di ERG scende; il valore stabile viene utilizzato per creare un guadagno netto in USD. Al momento del riscatto, il valore stabile può essere riscattato per una posizione ERG più ampia. Non solo hanno accresciuto la loro posizione in USD, ma hanno anche accresciuto la loro posizione in ERG.
- Quando SigmaUSD diventa un percorso di valore generativo oltre lo short, incentiva gli utenti a interagire con il protocollo AgeUSD su ERG.
- Il risultato di ciò sarà un sano sistema di riserva che favorisca la crescita attraverso l'interazione e lo scambio.
- A questo punto, aspettati l'apprezzamento in SigmaRSV. Aspettati che il tesoro cresca.

Questa è la principale barriera da superare, la commissione del 2,5%.

A parità di condizioni, questa è una barriera molto bassa al successo.
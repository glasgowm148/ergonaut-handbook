---
title: Yield
description: Consigue yield con tus ERG
published: true
date: 2022-01-22T02:35:07.751Z
tags: yield, staking
editor: markdown
dateCreated: 2022-01-22T02:17:01.506Z
---

# Consiguiendo Yield

Ergo es una cadena de bloques **Prueba de trabajo**, es decir, PoW. Por lo tanto, no es posible hacer staking en Ergo como lo haría en una cadena de bloques de **Staking**. Sin embargo, es posible obtener algún rendimiento de su ERG con Ergo en fondos de liquidez, tokenización de dApps, bots comerciales, plataformas de préstamos y otros mecanismos.


# Staking

Varios proyectos planean lanzar tokens nativos en Erg y planean ofrecer staking.

## [ErgoPad](https://ergopad.io/)

El propósito de ErgoPad es ayudar a los nuevos proyectos a generar capital a través de la venta de tokens durante las IDO u "ofertas iniciales descentralizadas" de tokens. ErgoPad ha implementado su propio token a través de un IDO que brinda a los inversores poderes de gobierno, así como la capacidad de stakear el token. Si los inversionistas alcanzan un determinado nivel de participación, pueden disfrutar de un acceso temprano a las ventas de semillas (a menudo a un precio más bajo que el que se cobrará en el IDO) para nuevos proyectos.

**Comunidad**
* [Discord](https://discord.gg/JdfVv7jp6b)
* [Twitter](https://twitter.com/ErgoPadOfficial)
* [Reddit](https://www.reddit.com/r/ergopad/)

<br>

# Creadores de mercado automatizados

Un Market Maker Automatizado (AMM) utiliza modelos matemáticos para establecer el precio y emparejar compradores y vendedores en lugar de simplemente emparejar órdenes de compra y venta, como en los libros de pedidos tradicionales. AMM es mejor en mercados con baja liquidez.

Una de las características de AMM es que los proveedores de liquidez agregan activos al intercambio por una tarifa, y el mercado se beneficia de un aumento en la liquidez, menor latencia, deslizamiento de precios limitado y menor volatilidad del mercado al usar esta liquidez adicional.

Pero debes estar al tanto del [impermanent loss](https://ergonaut.space/es/Guides/yield#impermanent-loss).

<br>

## [ErgoDex](https://ergodex.io/)

![screenshot_2022-01-09_at_18.13.43.png](/screenshot_2022-01-09_at_18.13.43.png)
Actualmente hay un intercambio descentralizado en Ergo, Ergodex. Hay varios grupos en ErgoDex con un porcentaje de rendimiento anual (APY) de activos estimado visible que se puede utilizar para la recolección de rendimiento.

Su monto canjeable cambia a medida que se usa el fondo común y el fondo gana un porcentaje de los intercambios. Obtienes un porcentaje de la tarifa del fondo proporcional a tu stake.

- SigRSV/ERG par
	-	Minimiza la pérdida impermanente (ambas monedas se mueven en la misma dirección en cuanto al precio)
- SigUSD/ERG
	- Alto riesgo de impermanent-loss, sin embargo, una inversión sólida si desea obtener tarifas de sus ahorros. SigUSD nunca ha estado cerca de perder su paridad.

**Comunidad**
- [Discord](https://discord.gg/KBrwstYcBx)
- [Telegram](https://t.me/ergodex_community)
- [Twitter](https://twitter.com/ErgoDex)
- [Reddit](https://www.reddit.com/r/ergodex/)
- [SigmaUSD Telegram](https://t.me/SigmaUSD)

<br>


### Swop.fi

- Pool de AMM

## Exchanges centralizados
Aunque no sin riesgo, hay varias opciones disponibles para obtener algunos rendimientos en su ERG.

### CoinEx

Hay un grupo AMM disponible en CoinEx.

# Trade Bots 

## KuCoin

KuCoin ofrece quizás las formas más simples de obtener rendimiento en su Erg con los siguientes bots disponibles:
- **Spot Grid** comercia con una cuadrícula que establece límites, vendiendo alto y comprando bajo. El problema es que si ERG va muy por encima de su rango, habrá vendido todo su ERG y se quedará con USDT. (vea: [impermanent loss](https://ergonaut.space/es/Guides/yield#impermanent-loss)).
- **Infinity Grid** funciona como el spot gridd pero no tiene un rango fijo
- **Futures Grid** lamentablemente todavía no está disponible para ERG.
- **DCA** reduce el riesgo de comprar caro invirtiendo a intervalos constantes.


**Comunidad**
- [ERG: Technical Analysis & Botting Telegram](https://t.me/ERGTechnicalAnalysis)

<br>

## Otros
En lugar de usar los bots en KuCoin, puede usar bots personalizados con un poco más de control sobre su estrategia comercial.
- 3commas
- shrimpy.io

# Fondos index

## [Ergo Index](https://ergo-index.fund/)

Ergo Index es una plataforma sin custodia que permite a los usuarios juntar sus fondos para invertir en una cartera de tokens en la cadena de bloques Ergo (todavía en desarrollo/no operativa).


- [GitHub](https://github.com/ergo-index)


## [Gate.io](https://www.gate.io/)

Puedes prestar allí por alrededor del 3,5%


# Anexo

## Impermanent Loss

La pérdida impermanente (IL) ocurre cuando la fórmula matemática de un AMM ajusta la relación de activos en un grupo para garantizar que ambos activos permanezcan en un valor uniforme.

Ejemplo: ingresa un grupo AMM de Erg/SigUSD, cuando los precios de cada uno de estos activos están en $10 y $1. Entonces, pones 1 Erg por cada $ 10 SigUSD en el pool.

Entonces, el precio de Erg sube a $20 un mes después. Supongamos que ganó $ 2 en tarifas. Entonces tendrá 0.8 Erg y $16 SigUSD para tener cantidades iguales en el grupo, o $32. Cuanto mayor sea el precio de Erg en relación con SigUSD, menos Erg tendrá.

Entonces, ¿por qué alguien proporcionaría liquidez a un AMM en un activo que esperaba aumentar y una moneda estable como SigUSD? La respuesta: recolección de volatilidades.

Los activos digitales como Erg no solo aumentan. Tienen mucha volatilidad, altibajos, y si está en un grupo de liquidez AMM, el equilibrio del AMM del grupo funciona como una especie de DCA en dólares. Compra más del activo que cuesta menos cuando está abajo y menos del activo que cuesta más cuando está arriba.


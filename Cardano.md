---
title: Cardano
description: 
published: true
date: 2021-03-23T23:17:00.267Z
tags: 
editor: markdown
dateCreated: 2021-02-25T07:53:55.991Z
---

Ergo Founded was by Charles Hoskinson’s *“favorite technologist”* Alex Chepurnoy who contributed to the development of Cardano and founded smartcontract.com (now Chainlink). In a interview Hoskinson described Ergo as;

> “one of the most revolutionary cryptocurrencies ever built. Got so many crazy ideas like non-outsourceable puzzles and sigma protocols and pruning the blockchain and roller chains. All this crazy stuff. Even has a proof of no premine.” — Charles Hoskinson
{.is-success}

The main objective of Ergo is to provide financial contracts in an efficient and secure way, so that people can use them in a decentralized manner and without any need for prior trust. The fully Cardano-compatible PoW can make great contributions to all developers in the Cardano ecosystem. Ergo is the first blockchain to adopt the smart contract language in the same eUTxO (extended UTXO) model as Cardano, enabling Proof of Work compatibility.

Although PoS is a very secure protocol, some smart contracts may require the consensus-theoretic security features of PoW for some part of their execution. The larger a dApp is, if it is doing collateralized DeFi, the larger the stake it has at its disposal, and since this is not yet fully resolved in the Proof of Stake consensus, it is a weak point. Ergo brings the proven security of PoW, with sufficient security for all more complex DApps implementations on top of the common UTxO model rather than trying to translate very natural cryptographic concepts inherent in PoW to PoS, where the game theory implications of the protocol are completely different.


1. Ergo will bring all the advantages of Proof of Work to users of the Cardano ecosystem.
1. Ergo is the first blockchain to adopt smart contract language similar to the UTxO model Cardano uses, bringing compatibility with Proof of Work to a whole new level.
1. Long-term scalability of dApps with the ability of parallelization of dApps.
1. More advanced cryptography with sigma protocols — highly flexible and composable cryptographic signatures.
1. The Ergo headless dApps framework.
1. Oracle pools — layered pools of pools of oracles with deviation checking consensus opening a whole new world of applications.
1. Local Exchange Trading System on top of Ergo.

# Oracle Pools

The oracle solution for Cardano will post data from Ergo’s oracle pools, treating the pre-processed data as a trusted source for its own records to the blockchain.

[Ergo vs Chainlink](https://www.ergoforum.org/t/oracle-pools-a-new-oracle-model/263)

[First steps towards interoperability with Cardano oracles](https://ergoplatform.org/en/blog/2020-11-09-first-steps-towards-interoperability-with-cardano-oracles/)

https://btcmanager.com/ergo-oracle-solution-cardano-ada-interoperability/

https://forum.cardano.org/t/ergo-will-complement-cardano/45412

https://emurgo.io/blog/emurgo-releases-oracle-core-for-developers

# Emurgo

**[EMURGO to Partner with Ergo and Build Blockchain-Based Decentralized Financial Solutions](https://emurgo.io/blog/emurgo-to-partner-with-ergo-and-build-blockchain-based-decentralized-financial-solutions)**
EMURGO’s strategic partnership with Ergo aligns with the objective to also meet the increasing needs for tailored decentralized financial (DeFi) solutions moving forward. As the interest in building decentralized financial services grows in tandem with the overall blockchain industry, this partnership allows for much-needed deeper research & DeFi solutions development. These solutions will explore the usage of Ergo’s smart contracts that are embedded with privacy features and interoperable with Cardano’s large global network. This will in turn, offer developers, investors, and interested parties the flexibility to utilize Ergo’s functionalities or to fully on-ramp onto larger blockchain ecosystems such as Cardano. 



# Cardano on StableCoins

**Cardano's Stablecoin Will be 'Better Than MakerDAO,' Says Hoskinson**
> "For example, we've partnered with Emrugo, and we're right now working on the logistics of a stablecoin with them that we're going to be building first on Ergo to verify everything works correctly, and then we'll pull it over into Cardano and this is going to be an algorithmic stablecoin," said Hoskinson, adding, "We think it'll be significantly better than MakerDAO."

**'Will SigmaUSD launch with gougen?**
>'  I'm going to see if we can do a SigmaUSD port after we do native-assets; we already have a Plutus implementation. We're discussing a lot of legal and regularatory stuff. It's a high priority of mine because it's interconnected for what we'd like to do for the next generation of Cardano, and it's very important to pull those things together.

**Charles answering '*are there use cases where PoW is better*'.**

>Until we deploy Orboros Genesis, PoW is significantly better and unique vs PoS in that you don't need a checkpoint, which is a huge advantage...and if you desire to gain a lot of computational abilities, especially with async resistance, PoW is better as you're building a supercomputer
>We are definitely going to do a stablecoin. It's just when you say stablecoin; there are many different types of stablecoins. You have things like asset-backed stablecoins where Tether (USDT) is an example of that, where someone buys USD, and they store in a bank account and then for every USD you mint a tether. You have commodity-backed stablecoins like goldcoins or these things... You have metastable coins where you take a basket of stablecoins, and you create a synthetic asset that's backed by that basket, and then you have algorithmic stablecoins like the Maker DAOs, where some mechanic keeps the coins stable, and then you have central bank issue digital currencies which is a sexy hot topic, like the Marshall Islands for example. There's a whole spectrum there, and actually, we have teams who look at each of these. In Africa, in particular, many governments have come to us and said, hey, we want to do commodity-backed stable coins.
>
> We're excited about that, and when we talk about sovereign counter partners, there I think the best thing to do is couple stable coins with universal basic income (UBI). Basically, during the operation of the stablecoin, there are transaction fees, and you let those fees accumulate in a sovereign wealth account and then what you do is you periodically give dividends to all the people of the country for that. This is super attractive when you have a smaller jurisdiction, let's say a Mauritius or something like that, and they have a lot of problems, and it allows them to basically get a lot of direct foreign investment and then they can do a direct distribution to their people.
We are exploring those, and there's been a lot of excitement on these governments' monetary policy side. The big challenge is also the regulatory layer on top of stablecoins. There needs to be the ability to freeze them, reverse transactions in the compliance layer. Cardano has a unique advantage here in that we have a product called Prism, and it's our identity management stack. It's blockchain agnostic, but it's tightly integrated with Cardano. It's a layer two identity stack based on DIDs, and this is going to enable people to have things like authenticated addresses where you could associate an address or an asset with a DID. DID is a decentralised identifier; then you can do KYC and AML on that DID, and then suddenly you can create a transitive graph of ownership and verify that all the people touching it has the right to do that. Who signs that DID is completely neutral. You could have a government sign it; regulatory bodies sign it; you can have a private entity like Pwc sign it or something like that.


# Articles
    
- [Ergo will complement Cardano](https://forum.cardano.org/t/ergo-will-complement-cardano/45412)
- There is another article [here](https://veriumfellow.medium.com/what-will-ergo-bring-to-cardano-2f7ae911a9bd) with a more technical overview of what Ergo brings to ADA.
- [https://thedailychain.com/hoskinson-cardano-working-on-stablecoin-to-rival-makerdao-developing-defi-products/](https://thedailychain.com/hoskinson-cardano-working-on-stablecoin-to-rival-makerdao-developing-defi-products/)
---
title: Cardano
description: 
published: true
date: 2021-05-15T11:18:43.542Z
tags: 
editor: markdown
dateCreated: 2021-02-25T07:53:55.991Z
---

> [F5: Scale-UP Cardano's DeFi Ecosystem - ErgoDex Plutus Port ](https://cardano.ideascale.com/a/dtd/ErgoDex-Plutus-Port/352410-48088)
{.is-info}

- [Ergo's Efficiency and interplay with PoS - Discussion](https://www.reddit.com/r/cardano/comments/nbdism/ergos_efficiency_and_interplay_with_pos/)
# Overview
Ergo was founded by Charles Hoskinson’s *“favorite technologist”*,  Alex Chepurnoy - who contributed to the development of Cardano and founded smartcontract.com (now Chainlink). In an interview, Hoskinson described Ergo as;

> “one of the most revolutionary cryptocurrencies ever built. Got so many crazy ideas like non-outsourceable puzzles and sigma protocols and pruning the blockchain and roller chains. All this crazy stuff. Even has a proof of no premine.” — Charles Hoskinson
{.is-success}

The main objective of Ergo is to provide financial contracts efficiently and securely so that people can use them in a decentralised manner and without any need for prior trust. The fully Cardano-compatible PoW can make significant contributions to all developers in the Cardano ecosystem. Ergo is the first blockchain to adopt the smart contract language in a similar eUTxO (extended UTXO) model as Cardano, with NiPoPoWs to enable compatibility. 

1. Ergo will bring all the advantages of Proof of Work to users of the Cardano ecosystem.
1. [ErgoDex](https://ergonaut.space/ergodex.pdf?11)
1. Ergo is the first blockchain to adopt smart contract language similar to the UTxO model Cardano uses, bringing compatibility with Proof of Work to a whole new level.
1. Long-term scalability of dApps with the ability of parallelisation of dApps.
1. More advanced cryptography with sigma protocols — highly flexible and composable cryptographic signatures.
1. The Ergo headless dApps framework.
1. Oracle pools — layered pools of oracles with deviation checking consensus opening a whole new world of applications.
1. Local Exchange Trading System on top of Ergo.

## Resources
    
- [Ergo will complement Cardano](https://forum.cardano.org/t/ergo-will-complement-cardano/45412)
- There is another article [here](https://veriumfellow.medium.com/what-will-ergo-bring-to-cardano-2f7ae911a9bd) with a more technical overview of what Ergo brings to ADA.
- [hoskinson-cardano-working-on-stablecoin to rival makerdao developing defi products](https://thedailychain.com/hoskinson-cardano-working-on-stablecoin-to-rival-makerdao-developing-defi-products/)
- [Special Announcement by Nico, Seba, and Robert | Cardano Live #18
](https://youtu.be/5oKMOVNyWxs?t=1968)


# Staking Pitfalls

Those that are familiar with the Lindy effect, which is often linked to Bitcoin’s monetary evolution, will recognize this process. The Lindy effect states that a technology’s remaining life expectancy is proportional to its current age, meaning that the longer it exists, the more its trusted to continue to exist. This means it’ll take time for Cardano’s young system to be trusted — particularly in comparison to Bitcoin that already abides resiliently for over 10 years with 99.98% up-time and zero known immutability breaches. The rigorous academic basis of Cardano is arguably the best possible foundation to build on, but it still needs to prove it is resilient against attacks ‘in the wild’ and thus undergo the test of time to earn the trust of investors. To justify an increasing ADA price that is important in Cardano’s security proposition, it is essential that the system will actually be used. It is therefore no coincidence that this is exactly what IOHK, Emurgo and the Cardano Foundation are focusing on.

Although PoS is a very secure protocol, some smart contracts may require the consensus-theoretic security features of PoW for some part of their execution. The larger a dApp is if it is doing collateralised DeFi, the more significant the stake it has at its disposal, and since this is not yet fully resolved in the Proof of Stake consensus, it is a weak point. Ergo brings the proven security of PoW, with sufficient protection for all more complex DApps implementations on top of the standard UTxO model rather than translating very natural cryptographic concepts inherent in PoW to PoS, where the game theory implications of the protocol are entirely different.



- [How Secure is Cardano?](https://medium.com/@undersearcher/how-secure-is-cardano-5f1e076be968)



# Emurgo

**[EMURGO to Partner with Ergo and Build Blockchain-Based Decentralised Financial Solutions](https://emurgo.io/blog/emurgo-to-partner-with-ergo-and-build-blockchain-based-decentralized-financial-solutions)**
EMURGO’s strategic partnership with Ergo aligns with the objective to also meet the increasing needs for tailored decentralised financial (DeFi) solutions moving forward. As the interest in building decentralised financial services grows in tandem with the overall blockchain industry, this partnership allows for much-needed deeper research & DeFi solutions development. These solutions will explore the usage of Ergo’s smart contracts that are embedded with privacy features and interoperable with Cardano’s extensive global network. This will, in turn, offer developers, investors, and interested parties the flexibility to utilise Ergo’s functionalities or to fully on-ramp onto larger blockchain ecosystems such as Cardano. 

## Oracle Pools

The oracle solution for Cardano will post data from Ergo’s oracle pools, treating the pre-processed data as a trusted source for its records to the blockchain.


Although Ergo adopts the PoW mechanism while Cardano adopts the PoS mechanism, they are highly compatible because both are based on eUTXO models. Ergo will bring Cardano the advantages of PoW, for instance, NiPoPoW, which supports ultra-light clients and cross-chain interoperability, because NiPoPoW cannot be used on PoS, and Cardano cannot use the technology directly but can use it via Ergo’s PoW to support ultra-light clients. Furthermore, Cardano has adopted Ergo's oracle pool scheme instead of Chainlink. The advantage of the oracle pool model is that no oracle tokens are issued so that the end-users can use the oracle services at an extremely low cost, and another advantage is that its data sources are decentralised and more reliable. Currently, Ergo oracle pools have two use cases, namely ERG/USD Oracle Pool and ADA/USD Oracle Pool. For details, please refer to the article "Deep Interpretation: What Ergo Will Bring to Cardano".


- [Ergo vs Chainlink](https://www.ergoforum.org/t/oracle-pools-a-new-oracle-model/263)
- [First steps towards interoperability with Cardano oracles](https://ergoplatform.org/en/blog/2020-11-09-first-steps-towards-interoperability-with-cardano-oracles/)
- [BTCManager: Ergo Oracle Solution Cardano ADA Interoperability](https://btcmanager.com/ergo-oracle-solution-cardano-ada-interoperability/)
- [Cardano Forums: Ergo Will Compliment Cardano](https://forum.cardano.org/t/ergo-will-complement-cardano/45412)
- [Emurgo: Emurgo releases oracle core for developers](https://emurgo.io/blog/emurgo-releases-oracle-core-for-developers)

# ErgoDex

ErgoDex is currently live on Ideascale [F5: Scale-UP Cardano's DeFi Ecosystem - ErgoDex Plutus Port ](https://cardano.ideascale.com/a/dtd/ErgoDex-Plutus-Port/352410-48088)

It will offer the first truly decentralised exchange, available across the Ergo and Cardano network. 


# StableCoin

The economic model for SigmaUSD (The AgeUSD Protocol) was created in joint partnership between IOHK, Emurgo and Ergo. While SigmaUSD.io uses ERG as it's BaseCoin, the Plutus port will use ADA. However the details of this implementation are still unclear. 


**Cardano's Stablecoin Will be 'Better Than MakerDAO,' Says Hoskinson**
> "For example, we've partnered with Emurgo, and we're right now working on the logistics of a stablecoin with them that we're going to be building first on Ergo to verify everything works correctly, and then we'll pull it over into Cardano and this is going to be an algorithmic stablecoin," said Hoskinson, adding, "We think it'll be significantly better than MakerDAO."

**'Will SigmaUSD launch with gougen?**
>'  I'm going to see if we can do a SigmaUSD port after we do native-assets; we already have a Plutus implementation. We're discussing a lot of legal and regularatory stuff. It's a high priority of mine because it's interconnected for what we'd like to do for the next generation of Cardano, and it's very important to pull those things together.

**Charles answering '*are there use cases where PoW is better*'.**

>Until we deploy Orboros Genesis, PoW is significantly better and unique vs PoS in that you don't need a checkpoint, which is a huge advantage...and if you desire to gain a lot of computational abilities, especially with async resistance, PoW is better as you're essentially building a supercomputer



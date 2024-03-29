---
title: FAQ
description: 
published: true
date: 2022-09-20T06:59:16.820Z
tags: 
editor: markdown
dateCreated: 2021-02-24T09:09:29.612Z
---

## Why Proof-of-Work ?

Ergo is based on the [Autolykos](/en/Glossary/Autolykos) Proof-of-Work protocol. 

Proof-of-Work (PoW) has tried and tested methods, and provides several benefits over Proof-of-Stake (PoS). You can see Charles Hoskinson discussing some of those benefits in a [recent AMA (timestamped)](https://youtu.be/Y27Q3wL_Hko?t=207)

Although PoS is a very secure protocol, some smart contracts may require the consensus-theoretic security features of PoW for some part of their execution. The larger a [dApp](/en/Glossary/dApps) is, if it is doing collateralized DeFi, the larger the stake it has at its disposal, and since this is not yet fully resolved in the Proof of Stake consensus, it is a weak point. Ergo brings the proven security of PoW, with sufficient security for all more complex DApps implementations on top of the common UTxO model.  The PoW+UTXO model was chosen, rather than trying to translate very natural cryptographic concepts inherent in PoW to PoS, where the game theory implications of the protocol are completely different.

- See our post on [Cardano](https://ergonaut.space/en/Ergo/Ergo-And-Cardano) for more information
- [Ergo: Why Proof of Work?](https://curiaregiscrypto.medium.com/ergo-why-proof-of-work-47c9b25fae70)
- [Entering the Next Era of Pow With Ergo](https://curiaregiscrypto.medium.com/entering-the-next-era-of-pow-with-ergo-e4d83530410c)
## Why was non-outsourceability turned off?

Autolykos v1 originally had non-outsourceability built-in to prevent mining pools on Ergo. However, it became apparent that with smart contracts, it's basically impossible to prevent pools. So, they  (the miners) turned it off so that not only larger players were able to take advantage of the loophole. Ergo is now focusing on memory hardness in an attempt to keep mining as fair as possible, which should help prevent ASICs mining at least. There are also some improvements for pooling, e.g. Stratum 2 protocol. 


> “Bypassing Non-Outsourceable Proof-of-Work Schemes Using Collateralized Smart Contracts” https://ia.cr/2020/044 was presented by Alex Chepurnoy at WTSC workshop associated with Financial Cryptography and Data Security 2020 in Malaysia
{.is-info}


- It's also discussed here on 'Unblocked with Robert Kornacki' [(14:45)](https://www.youtube.com/watch?v=2sbTMrQwWOw&feature=youtu.be)

Mining pools have certain benefits that are just now being exposed by Ergo, like more equitable token distribution for dApps/ projects. This is now available to miners on GETBLOK.io, using the world's first *working* SmartPools/subpooling system.
## What about 51% attacks?

Mining pools offer a buffer against such network attacks as the hash rate is distributed across thousands of individual miners.

The memory hardened aspect of ergo also makes this vector of attack more expensive as there is no ASIC support to rent. With the collective rentable rigs at the moment this isnt a viable path to a 51% attack. In theory, someone could build a massive GPU farm to try to launch such an attack. If a bad actor can rent a warehouse of ASIC and mine on a small chain with 51% attacks are a viable option... if there is an offramp. 

Usually, this attack is done for profit and there is massive dumping that occurs on an exchange as it is occuring. Meaning the attacker is going to dump tokens on an exchange then "double-spend" them back into their wallet. The current exchange situation doesn't provide the liquidity for a viable offramp. The rentable ASIC support isn't an option. So is it possible, in theory, yes, practical or likely I dont think so at all.

Ethereum classic is perhaps a bad example, as it shares the same mining algorithm as Eth. One could buy more than 100% existing hashrate of eth classic on NiceHash. It's not the same case for Ergo. Ergo also believes in the 'Good Miner' principle, In the case of Bitcoin - it was a good thing 51% existed. 

## Can I mine Erg?

Yes! But first you will need a dedicated GPU (AMD/Nvidia), see [mining](https://ergonaut.space/en/Guides/Mining) for more details.


# Use-Cases 

**The following quote was in response to a question about Ergo's **use cases**. Please see [FMFW x Ergo AMA](https://sigmanauts.medium.com/fmfw-x-ergo-ama-august-19-ee70af0d3f7e) for complete AMA discussion with kushti and Armeanio.** 

**"Ergo is an L1 (Layer 1) and we have a lot of applications already deployed by the community or in progress. Stablecoins, oracle pools, decentralized auction, decentralized DEX AMM pools, decentralized grid trading, decentralized options, tens of NFT projects, games, liquidity provision for fees to be paid in custom tokens, bridges, etc**

 **I am not capable to follow all the developments in the community even!"** -kushti


- Ergo's [use-cases](https://ergonaut.space/en/Ergo/Use-Cases) detailed

- Explore [Sigmaverse.io](https://sigmaverse.io) to see Ergo's entire dApp universe 

## [dApps](/en/dApps/dApps) 

- [ErgoMixer](/en/dApps/ErgoMixer)
- [ErgoAuctions](/en/dApps/ErgoAuctions)
- ErgoUtils
- [ErgoRaffle](/en/dApps/ErgoRaffle)


**Browse full list of Ergo dApps (decentralized applications) on [SigmaVerse.io](https://sigmaverse.io/all-projects/?category=All)**
## [SigmaUSD](/en/dApps/SigmaUSD/Overview)

Algorithmic Stablecoin, backed by a reserve which in it's most simplest form is betting long and short bets against each other. See [SigmaUSD](https://ergonaut.space/en/dApps/SigmaUSD/Overview) for more.

## [Spectrum](/en/dApps/ergodex)  (formerly ErgoDex)



**[Spectrum.DEX](https://app.spectrum.fi/ergo/swap) is a non-custodial decentralized exchange that allows a quick, effortless, and secure transfer of liquidity inside and between the Ergo and Cardano networks. The eUTXO model gives the unique possibility to have shared liquidity among different networks. Spectrum.DEX will eventually feature a full AMM, Order Book and more.**

Spectrum.DEX is an open-source DeFi product which take a part in both Ergo and Cardano platforms and as a consequence exists for purposes of both communities.

## Oracle Pools
There's a solid comparison of Oracle Pools on Ergo vs Chainlink given on the [ergoforum](https://www.ergoforum.org/t/oracle-pools-a-new-oracle-model/263) (by Robert Kornacki, Head of Research @ Emurgo).


- See our detailed article on [Oracle-Pools](https://ergonaut.space/en/Glossary/Oracle-Pools) for more.
- [Is the Ergo Oracle Sleeper the Next Chainlink?](https://www.reddit.com/r/AltStreetBets/comments/kfxst7/is_the_ergo_oracle_sleeper_the_next_chainlink/)
- [A new Cardano-based project is handling oracles a lot differently than Chainlink](https://cointelegraph.com/news/a-new-cardano-based-project-is-handling-oracles-a-lot-differently-than-chainlink)



# Background

## What are the basics?

The cryptographic part of Ergo script is based on sigma protocols and naturally supports threshold m-of-n signatures, ring signatures and more. Keeping all this in mind, we expect ErgoScript and Ergo’s design to make it uniquely useful as Contractual Money with countless applications possible. Ergo DApps and offchain protocols may be implemented in a truly decentralized way due to light clients.

For more fundamental changes Ergo is following a soft-forkability approach --- if an overwhelming majority of the network accepts a new feature, it is activated, however, old nodes which do not upgrade continue to operate normally and just skip over this feature validation. Thus disruptive hard forks should not be required in Ergo.

Ergo mining will always be stable, unlike Bitcoin and other PoW currencies, in which mining may become unstable after the emission period. Second, state size growth becomes controllable and predictable reducing hardware requirements for Ergo miners. Third, by collecting storage fees from outdated boxes, miners return lost coins to circulation preventing a steady decrease of circulating supply due to lost keys. To achieve survivability, Ergo provides economic improvements in addition to the technical ones, most central of which is a storage fee component which plays an important role for Ergo‘s stability.

All cryptocurrencies rely on contributions from the scientific research community. Gladly Ergo brings it in the core! 


## What is the Ergo Foundation? 

The Ergo Foundation is a community-driven entity focused on:
1. Promoting non-breaking development of Ergo Platform protocol;
1. Promoting the widespread adoption and use of Ergo Platform and its native token (ERG);
1. Developing the ecosystem around the Ergo Platform;
1. Promoting the use of Ergo Platform and blockchain technology for social good;
1. Supporting truly decentralized infrastructure, and;
1. Supporting privacy as a basic human right.

The Treasury’s allocation of Ergs is equivalent to 10% of the total block reward over the first 2 years and leaves miners with a block reward of 67.5 Ergs per block. After 2 years, the Treasury will continue to receive the part of the block reward that exceeds 67.5 Erg, however, this will be 0 after year 2.5 when the block reward becomes 66 Ergs per block.

- More information on [ergoplatform.org](https://ergoplatform.org/en/foundation/) and [Emission Schedule](https://ergoplatform.org/en/blog/2019_05_20-curve/)


## Why 'Ergo'? 

“Ergo means “therefore” in Latin, but “work” in Greek. I prefer the second meaning, but both are fine. Initially the name was chosen to point to the fact that the design of the cryptocurrency is ERGOnomical.”


## What is 'EFYT'

To fund development, promotion, events, to swap Ergo’s Ergo First Year Tokens (“EFYT”, further discussed below) into Ergs and to fund other activities which may advance the platform, Ergo has in place a Treasury which will receive 4.43% of the Ergs released during emission. During the first 2 years post‐mainnet launch, the Treasury will receive 7.5 Ergs per block. Given that the block reward for each block is 75 Ergs total, the Treasury’s allocation of Ergs is equivalent to 10% of the total block reward over the first 2 years and leaves miners with a block reward of 67.5 Ergs per block. After 2 years, the Treasury will continue to receive the part of the block reward that exceeds 67.5 Erg, however, this will be 0 after year 2.5 when the block reward becomes 66 Ergs per block. Readers familiar with some other PoW protocols with a Treasury, such as ZCash, may find this to be similar, however, it should be noted that the amount of Ergs going to the Treasury comprise a total of only 4,330,791.5, or 4.43% of the total monetary base, and is completed in just 2.5 years. This compares with ZCash’s Treasury, which was 10% of the ZCash total monetary base and 20% of all issued ZCash coins during the first 4 years. With Ergo, it is hoped that by 1 year post‐mainnet launch, Ergo will have achieved a high level of decentralization with a diverse developer, miner and user base. For the first year, the Treasury will be used for swapping of the EFYT on the Waves platform for Erg. For the remaining 1.5 years, a community voting mechanism will be put in place to determine how Treasury funds are spent.

> "The current distribution of EFYT can be found [here](http://dev.pywaves.org/assets/725Yv9oceWsB4GsYwyy4A52kEwyVrL5avubkeChSnL46). It should be noted that the max supply of EFYT is 1,970,945.0. This is 10% of the first year of Ergo token emission and the same number of Ergs that the Treasury will receive, meaning that the Treasury will have received 1,970,945.0 Ergs during year 1, sufficient to swap the max supply of EFYT for Erg."
>
>For more info please see: **https://ergoplatform.org/en/blog/emission/**
{.is-info}


## Where can I buy Erg?

- ergoplatform.org **#Exchanges** 

**https://ergoplatform.org/en/get-erg/#Exchanges**


## Where can I store Erg?

- ergoplatform.org **#Wallets** 

**https://ergoplatform.org/en/get-erg/#Wallets**

## How can I stake my Erg?
Ergo is a PoW (**Proof of Work**) coin not a PoS (**Proof of Stake**), which means that blocks are validated by miners, not by stakers, therefore you can't stake Erg directly.

However, it is possible to earn some yield from your ERG in combination with Ergo in liquidity pools, tokenisation of dApps, trading bots, lending platforms, and other mechanisms. 

You can 'stake' native tokens on Ergo in some form (on ergopad.io *live*, Night Owl Casino *soon*, ErgoMixer *soon*,+ more)  

For more info on earning off your Erg take a look at the [Yield guide](https://ergonaut.space/en/Guides/yield).


# Your Questions Answered

Any other questions? Comment below so we can expand this page !

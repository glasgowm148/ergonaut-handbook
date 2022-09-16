---
title: ErgoDocs/Mining
description: adapted from https://docs.ergoplatform.com/mining/
published: false
date: 2022-09-16T07:00:34.126Z
tags: mining, penambang, miner, gpu, mining, guides
editor: markdown
dateCreated: 2022-09-16T06:53:06.922Z
---

> There are active miner communities on [Discord](https://discord.gg/Q86PNMwRsu) and [Telegram](https://t.me/ergo_mining).
{.is-info}

# Mining

Ergo mining is based on [Autolykos](/en/Glossary/Autolykos), an ASIC resistant Proof of Work algorithm written in Scala that runs cool and increases mining equipment longevity. Combined with the [eUTXO](/en/Glossary/eUTXO) model, this creates a highly efficient Proof of Work. Ergo had a fair launch with no premine, ICO or VC funding. 

**Getting Started**

Unless you have 1TH/s+, you likely want to be mining from a pool. Available miners and pools listed in the pool section. 

- [Mining from a pool](https://docs.ergoplatform.com/mining/setup/join)
- [Solo Mining](https://docs.ergoplatform.com/mining/setup/solo)
- [Hosting a pool](https://docs.ergoplatform.com/mining/setup/pool)
- [Subpooling](https://docs.ergoplatform.com/mining/setup/subpool)

**Resources**

- The [Ergo Explorer](https://explorer.ergoplatform.com) can give you various information & stats on mining and the network. 
- [Difficulty and epoch monitor.](http://cds.oette.info/ergo_diff.htm)
- [Wallets](https://ergoplatform.org/en/get-erg/#Wallets)

## [Autolykos](/en/Glossary/Autolykos)

- Autolykos v1 originally had pool-resistance built-in through the use of non-outsourceable puzzles.
- **The Hardening Hard-Fork** on block `417,792` marked the launch of Autolykos v2, enabling mining pools. See this [paper](https://ia.cr/2020/044). 
- [**EIP27:**](https://github.com/ergoplatform/eips/blob/master/eip-0027.md) was passed with overwhelming community support, extending emission by 4,566,336 blocks (~17.38 years). This was activated on block `777217`


## [Governance](/en/Guides/Mining/Voting)

Ergo Miners have the ability to adjust the block size which increases the amount of transactions per block. This increases potential rewards but also adds additional storage requirements. adjust the emission macroeconomics, meaning the long term economic security of the protocol is up to miners to decide. 

In addition to the protocol parameters above that can be changed via on-chain miner voting, most things on Ergo can be changed via a soft-forking protocol (90% support required). This excludes critical changes such as changing the max supply. 


## [Storage Rent](/en/Glossary/Storage-Rent)



Storage Rent is a nominal fee (.14ERG per 4 years from an unmoved box) + transaction fees.

The problem with “storage rent fee” is this “fee” part — which may look like a disadvantage. However, programmers can quickly realize the importance of it by just imagining life without garbage collection in their language of choice.

> *Claiming fees sound great… But what happens if a UTXO cannot pay the fee?*

Miners can take over assets inside a UTXO if there are not enough ERGs to pay for rent. This feature is one of the most interesting reward mechanisms a PoW blockchain can offer miners. The relevance of this is particularly important in a blockchain that has the capacity to have a wide variety of assets.

As Ergo matures, more revenue streams will become available to miners. 

- Sidechain Rewards
- Bridge Infrastructure
- L2 Infrastructure

## Getting Started

Search your card here on the [Autolykos v2 hashrates spreadsheet](https://docs.google.com/spreadsheets/d/1NsuoDB27EwCo_BlSjCP3GMLfTSJRPIWIBsL-wPTllUg) to find your estimated hashrate.

There are various pools available as seen on [miningpoolstats.stream/ergo](https://miningpoolstats.stream/ergo)

## Miners

You can use multiple miners to mine Ergo (Autolykos2). Below you will find a list of mining software used to mine ERG. There are various opinions on which mining software is best, and some are clear winners. The best advice is to try them all and see what works best for you.

In addition to dedicated mining software, there are also Mining OS or operating systems such as HiveOS, one of the more popular options. This allows you to control your rig through dedicated software that will assist with connecting to pools, OC settings, and miners or mining software. These would be considered an all in one package, whereas using a specific miner may require other resources or plugins.

###  Software:

- [Lolminer](https://github.com/Lolliedieb/lolMiner-releases)
- [Nanominer](https://github.com/nanopool/nanominer/releases)
- [NB Miner](https://github.com/NebuTech/NBMiner)
- [SRB Miner](https://github.com/doktor83/SRBMiner-Multi/releases)
    - [SRBMiner-MULTI - How to mine Ergo coin (autolykos2)](https://www.youtube.com/watch?v=thBPstQJVWo)
- [Team Red Miner](https://github.com/todxx/teamredminer/releases)
- [Trex Miner](https://github.com/trexminer/T-Rex/releases)

### Source Code Miners

- [AMD miner](https://github.com/mhssamadani/Autolykos2_AMD_Miner)
- [Nvidia miner](https://github.com/mhssamadani/Autolykos2_NV_Miner)

### Other Miners

- [CUDA-based GPU miner for Ergo](https://github.com/ergoplatform/Autolykos-GPU-miner) for NVidia cards
- [OpenCL miner for ERGO](https://github.com/mhssamadani/ergoAMDminer) for AMD cards 
- [#smartpools](https://discord.gg/qdEpkRQZ4P) 

### Operating Systems

- [Hive OS](https://hiveos.farm/)
    - [Mining Ergo on HiveOS](https://ergoplatform.org/en/blog/2022-03-22-mining-ergo-on-hiveos/)
    - [Mining Ergo on Windows](https://ergoplatform.org/en/blog/2022-03-17-mining-ergo-on-windows/)
- [Minerstat](https://minerstat.com/)
- [Rave OS](https://raveos.com/)
- [Simple Mining OS](https://simplemining.net/)

### [Nice Hash](https://www.nicehash.com/) 
- [NiceTalk live with Ergo](https://www.nicehash.com/blog/post/join-us-live-with-ergo-on-nice-talk-on-the-29th)




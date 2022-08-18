---
title: The Complete Ergo Mining Handbook v2.0
description: Some 3rd party pages link to this non-existent URL path
published: true
date: 2022-08-18T21:56:55.626Z
tags: 
editor: markdown
dateCreated: 2022-08-11T20:02:32.669Z
---

```plaintext
# **The Complete Ergo Mining Handbook v2.0**

![5e8765a7-6344-4a81-b283-87c695056ef6.jpeg](/5e8765a7-6344-4a81-b283-87c695056ef6.jpeg =x350)

> There are active miner communities for Ergo on [Discord](https://discord.gg/Q86PNMwRsu) and [Telegram](https://t.me/ergo_mining). For direct support there's #mining-support on Discord - Enable the mining role in #get-roles. 
{.is-info}

- [Mining Ergo on HiveOS](https://ergoplatform.org/en/blog/2022-03-22-mining-ergo-on-hiveos/)
- [Mining Ergo on Windows](https://ergoplatform.org/en/blog/2022-03-17-mining-ergo-on-windows/)

## The Coin: What is Ergo?

Ergo has a strictly limited supply, Ergo's original 8 year emission schedule was extended by miners with EIP-27 (live since block #777,217) while maintaining original max supply. All $ERG tokens are mined through an original Proof‐of‐Work (“PoW”) algorithm called Autolykos v2, designed to be ASIC resistant, which employs a [smoothed difficulty algorithm](https://ergoplatform.org/docs/ErgoPow.pdf).

Miners have to perform memory-hard computations~(at least 2.5 GB memory is currently needed but the  most efficient implementation utilizes around 4 GB of vRAM- *currently*) that makes Ergo friendly for GPU mining. A part of Ergo's ASIC resistance comes from Autolykos V2 increasing table size feature, this slowly increases the minimum memory requirements to GPU mine Ergo over time. 

There was 0 ERG in existence at launch of mainnet as there was no ICO nor pre‐mine. At the end of 8 years, the final Erg supply will be 97,739,925 Ergs. The Ergo block interval is 2 minutes and for the first 2 years, each block will release a total of 75 Ergs to be shared between the miners and the Treasury (Treasury discussed below). But starting at year 2, the rate of emission will fall by 3.0 Ergs and thereafter further decline every 3 months by an additional 3.0 Ergs, ~~which will result in an end to emission 8 years after launch.~~

> See [Ergo Emission: details, retargeting via a soft-fork](https://www.ergoforum.org/t/ergo-emission-details-retargeting-via-a-soft-fork/2778) and [EIP-27 github](https://github.com/ergoplatform/eips/blob/master/eip-0027.md) for kushti's soft-fork proposal in final implemented form. Original 8 year emission schedule has been extended after supermajority of miners vote in favor of soft fork. Total supply of 97,739,925 Ergs is strictly preserved.   
{.is-warning} 


- Check out the updated emissions curve, including EIP-27 re-emission contract with [ergo.watch/emission](https://ergo.watch/emission).

- The [explorer](https://explorer.ergoplatform.com) can give you various information & stats on mining and the network. 
- The [difficulty over time](https://explorer.ergoplatform.com/en/charts/difficulty) is visible here.
- [Difficulty and epoch monitor.](http://cds.oette.info/ergo_diff.htm)

For more information about Ergo follow the links below:

-   [Ergo Platorm](https://ergoplatform.org/en/)
-   [Ergo Basics](https://ergoplatform.org/en/basics/)
-   [Ergo Manifesto](https://ergoplatform.org/en/blog/2021-04-26-the-ergo-manifesto/)
-   [Ergo Whitepapers](https://ergoplatform.org/en/documents/)

## Bookmark This "official" Ergo Wallet 🔗  
### **https://ergoplatform.org/en/get-erg/#Wallets**
#### Yoroi is no longer a recommended Ergo wallet. If you check the official Ergo wallet link URL above, you will see some great "team" and "other" wallets, but no mention of Yoroi.  

- Yoroi went **from 1st to worst** Ergo  wallet?
Restore Yoroi balance on better alternatives using Import or Restore Wallet options, you will need correct mnemonic seed phrase of course.

A wallet will be required for you to collect your mining rewards. Digital wallets can help keep your digital currency safe, private and in your control. We highly recommend the use of wallets for storing Ergo assets (technically, they store the keys to your Ergo addresses). But keep in mind, your wallet is unlike your bank account, so take extra precautions with your passwords and be sure to perform regular backups to protect your money.

### Wallet Types:

[Third Party Wallets](https://docs.ergoplatform.com/dev/wallet/)

[Ergo Node Wallet](https://github.com/ergoplatform/ergo/wiki/Set-up-a-full-node)

-   [How to set up and configure a full Ergo node on Windows (Youtube)](https://www.youtube.com/watch?v=fpEDJ1CM6ns)

> Note that most wallets are supported by third parties, we only provide the information as a courtesy, in order to simplify the overall digital currency experience for you.
{.is-warning}


> Please don't mine direct to exchanges as this allows them to control price movement. Support decentralization.
{.is-danger}


## The Hardware:

You will need computer hardware to mine Ergo also refered to as a mining rig. Ergo mining is ASIC resistant and requires a GPU (Graphics Card) for mining. A mining rig can be as simple as a single GPU gaming computer, up to a multi GPU mining rig.

While it is possible to mine Ergo with a 4gb GPU. A 6GB GPU is the suggested minimum as Ergo heavily relies on memory usage while the core processor sits idle. 

> Note: this last statement is seemingly pre Ergo "hardening upgrade" (Ergo's only hardfork). As mentioned earlier in Handbook, 3gb is enough VRAM to mine Erg but that will soon change with Ergo's scheduled "DAG" increase [(DAG is a misnomer according to kushti here it's actually a table)](https://www.ergoforum.org/t/test-vectors-for-increased-n-values/2887) .
{.is-info} 

### Components required to build a mining rig:

-   [Graphics Card (GPU)](https://ergonaut.space/en/Guides/Mining/Graphics_Cards)


-   [Motherboards (MOBO)](/en/Guides/Mining/Motherboards)

-   Power Supply (PSU)
-   Processor (CPU)
-   Memory (RAM)
-   Storage (USB, SSD, HDD)
-   Other Hardware
    -   GPU Risers
    -   CPU Cooler
    -   Mining Rack
    -   Fans

Search your card here [Autolykos v2 hashrates](https://docs.google.com/spreadsheets/d/1NsuoDB27EwCo_BlSjCP3GMLfTSJRPIWIBsL-wPTllUg) to find the hashrate.

## The Pools:

![photo_2021-10-15_23-03-13.jpg](/photo_2021-10-15_23-03-13.jpg =x300)  
- Artwork by: Autolykos Megistos
---

### [GetBlok.io Smart Pool](https://ergo.getblok.io)
- [How to connect to GetBlok](https://www.getblok.io/how-to-connect/)
- [GetBlok Telegram Chat](https://t.me/getblok)
- [GetBlok Discord](https://discord.gg/h9uF3cNXdY)

### [LeafPool](https://ergo.leafpool.com/)
- [Getting started on LeafPool](https://ergo.leafpool.com/getting-started)

### [Enigma Pool](https://enigmapool.com/)
- [Getting started on Enigma Pool](https://enigmapool.com/getstarted) 

### [Miningcore](https://miningcore.pro/pool/ergo/)
- [Miningcore FAQ](https://miningcore.pro/faq)

### [WoolyPooly](https://woolypooly.com/en/coin/erg)
- [How to start mining Ergo (ERG) on Windows with AMD RX 4GB cards](https://www.youtube.com/watch?v=47eBVIjWYqY)
- [WoolyPooly Discord](https://woolypooly.com/discord)
- [WoolyPooly Telegram Chat](https://woolypooly.com/telegram)

### [K1pool](https://k1pool.com/pool/erg)
- [How to start mining on K1pool](https://k1pool.com/pool/erg/how-to-start)

### [2Miners](https://2miners.com/erg-mining-pool)
- [How to start mining Ergo](https://erg.2miners.com/help)


 ### [F2pool](https://www.f2pool.com/?_ga=2.253802568.1957310317.1634436769-1506845288.1634436769)
- [How to mine Ergo (ERG) on f2pool](https://f2pool.io/mining/guides/how-to-mine-ergo/)

### [FlyPool](https://ergo.flypool.org/)
- [How to connect on FlyPool](https://ergo.flypool.org/start)

### [HeroMiners](https://ergo.herominers.com/)

-   [Hero Miners: How to Mine Ergo (ERG)? Complete Beginner’s Guide](https://herominers.medium.com/how-to-mine-ergo-erg-complete-beginners-guide-608a87e89ed6)
-   [HeroMiners: How to mine Erg](https://ergo.herominers.com/#how-to-mine-ergo-erg)
-   [How to Mine Ergo? Step by Step (Youtube)](https://www.youtube.com/watch?v=4SnpCF67kyc)

---

Check pool stats to see ranking of pools. See note regarding 51% attack below

-   [Mining Pool Stats](https://miningpoolstats.stream/ergo)

> Please do not mine to mining pools with large hashrate. Any pool close to 51% of the total network is at risk of an attack.
{.is-warning}


-   [What about 51% attacks](https://www.reddit.com/r/ergonauts/comments/mgpnb7/51_attack_possibilities/) ?

## The Miners: (Mining Software)
There are multiple miners that can be used to mine Ergo (Autolykos2).  Below you will find a list of mining software that can be used to mine ERG.  There are various opinions as to which mining software is best and some are clear winners.  Best advice is to try them all if you can and see what works best for your rig set up specifically.   What works for one may or may not work for another.

In addition to dedicated mining software, there are also Mining OS or operating systems such as HiveOS, which is one of the more popular options.  This allows you to control your rig through dedicated software that will assist with connecting to pools, OC settings, and miners or mining software. These would be considered an all in one package where as using a specific miner may require other resources or plug ins.

![capture.jpg](/capture.jpg)
  [Image From r/Erg_Miners](https://www.reddit.com/r/erg_miners/comments/njmlfq/list_of_currently_used_miners_for_ergo_with/)

### Mining Software:
####	[Lolminer](https://github.com/Lolliedieb/lolMiner-releases)
#### [Nanominer](https://github.com/nanopool/nanominer/releases)
####	[NB Miner](https://github.com/NebuTech/NBMiner)
#### [SRB Miner](https://github.com/doktor83/SRBMiner-Multi/releases)
-   [SRBMiner-MULTI - How to mine Ergo coin (autolykos2)](https://www.youtube.com/watch?v=thBPstQJVWo)
#### [Team Red Miner](https://github.com/todxx/teamredminer/releases)
#### [Trex Miner](https://github.com/trexminer/T-Rex/releases)

### Mining OS:
#### [Hive OS](https://hiveos.farm/)
#### [Minerstat](https://minerstat.com/)

#### [Nice Hash](https://www.nicehash.com/) 
- [NiceTalk live with Ergo](https://www.nicehash.com/blog/post/join-us-live-with-ergo-on-nice-talk-on-the-29th)
#### [Rave OS](https://raveos.com/)
####	[Simple Mining OS](https://simplemining.net/)




## Source Code Miners

For the [AMD miner](https://github.com/mhssamadani/Autolykos2_AMD_Miner), the compatible Operating Systems are:

-   RedHat Enterprise Linux 7.2 (64-bit version)
-   RedHat Enterprise Linux 6.8 (64-bit version)
-   Ubuntu 16.04 (64-bit version)

Ergo can also be mined with [Nvidia miner](https://github.com/mhssamadani/Autolykos2_NV_Miner)

Miners can fix value by minting [SigUSD](https://sigmausd.io/#/)

[Start mining](https://git.io/fjqwp)


# Solo Mining

You can solo mine on any of the pools that offer a solo port.  Otherwise you will need to build a node and stratum server (pool) can also try [ergoNomp](https://github.com/btclinux/ergo-nomp)

Please check [this form](https://docs.google.com/forms/d/e/1FAIpQLScBFv3mxpu5Erv55zvfFuIo2NnaWht3cc70xZoRo-3c58Cv0A/viewform) to see if solo mining is worthwhile.


- [Autolykos2_NV_Miner](https://https://github.com/mhssamadani/Autolykos2_NV_Miner)
- [Autolykos2_AMD_Miner](https://github.com/mhssamadani/Autolykos2_AMD_Miner)

In order to operate them, you may or may not need to use Stratum Server and Stratum Proxy. These two projects are here:

- [ErgoStratumServer](https://github.com/mhssamadani/ErgoStratumServer)
- [ErgoStratumProxy](https://github.com/mhssamadani/ErgoStratumProxy)

# Difficulty 

Ergo uses the linear least square method which smoothes over 8 epochs (8 x 1024 blocks). This was designed to prevent malicious time warp and coin-hopping attacks.

The [difficulty over time](https://explorer.ergoplatform.com/en/charts/difficulty) is visible here. If you want an estimate of what might be next you can observe the [Difficulty and epoch monitor.](http://cds.oette.info/ergo_diff.htm)

# Host A Pool

Currently the [#host-a-pool](https://discord.gg/kxbrHVwnm5) on Discord is the best place to get support configuring a pool. 

- [ErgoStratumProxy](https://github.com/mhssamadani/ErgoStratumProxy) | Miner Connection + Work Management
- [ErgoStratumServer](https://github.com/mhssamadani/ErgoStratumServer) |  Pool Server
- [ergo-nomp](https://github.com/btclinux/ergo-nomp) | Node open mining portal configufed for ergo

**Step by Step**

1. Setup a Node
2. Setup ErgoStratumServer
3. Point [ergo-nomp](https://github.com/btclinux/ergo-nomp) to (1) and (2)


## Resources

**Calculators**

-   [ErgoPlatform - Mining Calculator](https://ergoplatform.org/en/mining/)
-   [Plutomonkey Calculator](https://pool.plutomonkey.com/)
-   [Miner Stats](https://minerstat.com/coin/erg)

**Other Miners**
- [CUDA-based GPU miner for Ergo](https://github.com/ergoplatform/Autolykos-GPU-miner) for NVidia cards
- [OpenCL miner for ERGO](https://github.com/mhssamadani/ergoAMDminer) for AMD cards 
- [#smartpools](https://discord.gg/qdEpkRQZ4P) 

<!-- Gives a 503 Service Unavailable Error on December 31, 2021, commented out. Leaving because I don't know if this is a temporary issue. @cafebedouin
- [ErgoPool - mining pool for self-sovereign Ergo miners!](https://ergopool.io/) -->



## Guides

-   [Mining $ERG: The Complete Guide](https://thecryptodrip.com/how-to-mine-erg-guide/)
-   [ErgoForum: Mining Ergo for Fun and Profit](https://www.ergoforum.org/t/mining-ergo-for-fun-and-profit/154)
-   [ErgoPlatform: Mining Ergo for Fun and Profit](https://ergoplatform.org/en/blog/2019_12_22_mining_for_fun/)
-   [ErgoForum: Q&A on mining (for pool operators and solo miner)](https://www.ergoforum.org/t/q-a-on-mining-for-pool-operators-and-solo-miners/587)

Credits [@ÅrÖhBê](https://t.me/arohbe) [@Glasgowm](https://t.me/glasgowm)
```
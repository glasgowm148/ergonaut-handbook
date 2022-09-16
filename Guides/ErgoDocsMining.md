---
title: ErgoDocs/Mining
description: adapted from https://docs.ergoplatform.com/mining/
published: true
date: 2022-09-16T07:52:45.004Z
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

# Solo Mining

You can solo mine on any pool that offers a solo port. Otherwise, you will essentially need to host your own pool.

Firstly, check out this [calculator](https://docs.google.com/forms/d/e/1FAIpQLScBFv3mxpu5Erv55zvfFuIo2NnaWht3cc70xZoRo-3c58Cv0A/viewform) if you're not sure if you should be solo mining.

There is now a solo-mining smart subpool on [getblok](https://www.getblok.io/smartpools/). Alternatively 2Miners, solopool.org and others offer Solo mining. 



## Getting Started

To solo mine you will need one of the following depending on your setup. 

- [Autolykos2_NV_Miner](https://https://github.com/mhssamadani/Autolykos2_NV_Miner)
- [Autolykos2_AMD_Miner](https://github.com/mhssamadani/Autolykos2_AMD_Miner)

You may or may not need to use Stratum Server and Stratum Proxy to operate them. These two projects are here:

- [ErgoStratumServer](https://github.com/mhssamadani/ErgoStratumServer)
- [ErgoStratumProxy](https://github.com/mhssamadani/ErgoStratumProxy)

To be able to spend any ERG mined this way, you will need to add this to your `.config`

```
ergo {
  wallet {
    checkEIP27 = true
  }
}
```

## Resources

- [Ergo Node + Stratum Server mining tutorial](https://www.youtube.com/watch?v=_1M8dGpfKjU)
- [Youtube: Mine Ergo from your own Node](https://www.youtube.com/watch?v=ubov4oweA20)
- [ErgoForum: Q&A on mining (for pool operators and solo miner)](https://www.ergoforum.org/t/q-a-on-mining-for-pool-operators-and-solo-miners/587)
# Hosting a Pool on Ergo

To host your own pool on Ergo you must first setup a local instance of the Ergo [node](https://docs.ergoplatform.com/node/node/) which should then point to your pool software ([Miningcore](https://docs.ergoplatform.com/mining/setup/miningcore) or [ErgoStratumServer](https://docs.ergoplatform.com/mining/setup/stratum))


> Community support available in [#host-a-pool](https://discord.gg/kxbrHVwnm5) on Discord.
{.is-info}


# Subpool
> subpooling is now live at [ergo.getblok.io/smartpool](https://ergo.getblok.io/smartpool)
{.is-success}




[ergo-subpooling](https://github.com/K-Singh/ergo-subpooling) is a smart contract based mining pool that allows groups of friends to pool together their hashrates in order to get mining pool rewards quicker than they would alone. Subpooling allows members to mine to the same address without worrying about one person controlling the funds. The goal of this dApp is to help encourage decentralization of mining pools while also promoting small time miners who may not be able to get block rewards fast enough on normal mining pools. This project was developed for ERGOHACK II.

# Autolykos

Autolykos, named after the Greek God Autolycus for the original non-outsourcability built-in in version one. However, it became apparent that pool resistance was infeasible due to large players having an advantage with smart contracts. ["Bypassing Non-Outsourceable Proof-of-Work Schemes Using Collateralized Smart Contracts"](https://ia.cr/2020/044) was presented by Alex Chepurnoy at the WTSC workshop associated with Financial Cryptography and Data Security 2020 in Malaysia.


**Autolykos V2** has the following modifications

- *non-outsourceable puzzles* were disabled. It turns out (based on more than one year of non-outsourceable PoW experience) that non-outsourceable PoW is not an attractive option for small miners.
- Now, the algorithm is trying to bind an efficient solving procedure with a single table of ~2 GB (initially), which significantly reduces memory optimisations possibilities
- Table size (memory requirements of a solving algorithm) grows with time
- The table depends solely on the block height, so there is no penalisation for recalculating block candidates for the same height

**Basic Ideas:**

- Like Autolykos-1, based on the k-sum problem, a miner needs to find `k (k=32)` out of `N (2^n = 2^26)` elements and the hash of their sum must be less than the target value (inverse of the difficulty)
- k indexes are pseudorandom values derived from block candidate and nonce
- N elements are derived from block height and constants, unlike Autolykos v.1, so miners can recalculate block candidates quickly now (so only indexes are depending on them)
- Indexes calculation also involving the same table (which elements are last 31 bytes of `H(i | | h | | M )`, where i is in [0, N), `h` is block height, M is padding to slow down hash calculation (8kb of constant data).

So algorithm tries to make mining efficient for ones that store the table, which is `2^26 * 31 = 2,080,374,784` bytes initially (about 2GB). Thus Autolykos is now is friendly to all the GPUs.

Also, table size (N value) is growing with time as follows. Until block `614,400`, `N = 2^{26} = 67,108,864 elements (31 bytes each)`. From this block, and until block `4,198,400`, every `51,200 blocks` `N` is increased by 5 percent. Since block `4,198,400`, value of `N` is fixed and equals to `2,143,944,600`. Test vectors for `N` values are provided in the paper.



## Difficulty Adjustment

Ergo uses the **linear least square method** to calculate difficulty. This function is based on the past eight epochs (1024 blocks), as described in [this paper](https://eprint.iacr.org/2017/731.pdf) to obtain the target block interval of 120s (2 minutes). (On average, during steady-hash). 

- [Coin hopping Attack — What after a month of Bitcoin hardfork?](https://medium.com/nikoin/coin-hopping-attack-what-after-a-month-of-bitcoin-hardfork-f5a92151fb7b)

Autolykos will adjust slowly in response to fluctuating hashrate, but this helps prevent **adversarial** hopping. This algorithm has a 1.9% error rate compared to bitcoins 9.1% error rate (exponential 10% hash rate growth). 

**Can it be quicker?**

Ergo already uses an epoch length of ~1.5 days (with normal block rate), compared to Bitcoin's two weeks. Having a quicker difficulty readjustment can lead to Timewarp attacks (amongst others). More epochs were considered, but the retargeting function is also non-linear, so it can adjust sooner than the linear function in certain popular scenarios; and it is unclear whether any hard-fork would be required at this stage. 

While the consistenty of payouts has not been ideal during price drops, and is more suited for larger hashrates. Changing it at this stage would require a hard-fork to change (and then a HF again to add it back at a larger hash - or some timed mechanism). 

So the general consensus is people would rather deal with the inconsistent rewards until the mining landscape is clearer. 


## Resources

- [Yellow Paper](https://www.docdroid.net/mcoitvK/ergopow-pdf)
- [ergo/src/main/scala/org/ergoplatform/mining/](https://discord.com/channels/668903786361651200/668903786902847502/990962713675055114)

### Test Vectors 

- [Test vectors for increased N values ](https://www.ergoforum.org/t/test-vectors-for-increased-n-values/2887/2)

### Solution Verification
```
Test Vectors - Ergo:
credit: Wolf9466#9466 on Discord

Height = 569806 (0x8B1CE)
Item count = 67108864 (0x4000000)
Prehash Item KAT:

Item index 0          : 0x00596fe417902d8fe61763deb06286d3bf787f3c8ea2cc3063724dd307993caa
Item index 4          : 0x00832cba40f67d525e9c449f17f46e3bfcdb663427d4289e35bc8e04b0c97765
Item index 255        : 0x003f44309d54120e5d41b36a245fea4098948f7e8c5c052247922b74a6c8e7b9
Item index 67108863    : 0x000701c3dd5db987aab0bb57f6e89ea9dbdc1dd88ffcac698bfde407d95063ce


Message = 0x9b8cb36a9b738fa3678521d00c938631e1a192bc1919f004d2cbabdaa33835b4
Nonce = 0x5d340003e9c460dc

Blake #1: 0xbd54dc777dc062c63b2f8cdd4d56f4f57b64d648420f62ef0e6f3935b0046fc99e7ea07b167ccadeaf2cd396504477697f5123e72887f61333358b5edbd5aa66

Blake #2: 0x6dbc710c2fb6e975d93af456686617b97595a0cec9dd22d57b8a7176d3f470b175eccfc1f97cecc13207fb68358c608930e5d7cfcdd0b3a4da8b9acb508e3248

Result = 0x0c3b54f29c8ac1a407f83cd09f3d61bc32996a3d58a7d9fe9fe0e0a08572e367f96b164cc3254ce5379622e007de97c76b1232030d899e0da83bc82e00000000
```
# Governance

Many parameters can be changed on-the-fly via miners voting, such as instructions costs, computational cost limit per block, block size limit, storage fee factor, block version, etc. 

Voting for the block version lasts 32 epochs and requires more than 90 percent of the miners to vote for the change. A simple majority is enough for less critical changes such as block size limit. We will further refer to the changes of the first kind as foundational changes, and we refer to the changes of the second kind as everyday changes. Per block, a miner can vote for two everyday changes and one foundational change, with the votes to be included in the block's header.

To vote **Yes** and propose a change in the first block of an epoch, a miner is publishing the identifier of the change directly in the block header. To vote **No** (or avoid voting at all, which is the same), a miner writes zero value instead of a corresponding byte (another option is to provide a vote identifier not considered within the epoch).

## System constants:

- Voting epoch length = `1024` blocks.
- Voting epochs per foundational change = `32`
- Voting epochs before approved foundational change activation = `128`


## Parameters table


The following table describes vote identifiers, default values (during launch), possible steps, and minimum and maximum values. If the step is not defined in the table, its value is defined as $\max(\lfloor current\_value / 100 \rfloor, 1)$. If the minimum value for a parameter is not defined, it equals zero. If the maximum value is not defined, it equals `1,073,741,823`.

A miner includes a parameter identifier ($id$) into the block header to propose or vote for increasing a parameter. If the miner supports decreasing the parameter, he includes ($-id$) into the block header.


| ID | Description | Default | Step | Min | Max |
|---|---|---|---|---|---|
| 1 | Storage fee factor (per byte storage period) | 1250000 | 25000 | 0 | 2500000 |
| 2 | Minimum monetary value of a box | 360 | 10 | 0 | 10000 |
| 3 | Maximum block size | 524288 |  | 16384 |  |
| 4 | Maximum cummulative computational cost of a block | 1000000 |  | 16384 |  |
| 5 | Token access cost | 100 |  |  |  |
| 6 | Cost per one transaction input | 2000 |  |  |  |
| 7 | Cost per one data input | 100 |  |  |  |
| 8 | Cost per one transaction output | 100 |  |  |  |
| 120 | Soft-fork (increasing version of a block) |  |  |  |  |

Parameter values are to be written into the extension section on the first block of a voting epoch,
that is, in the extension of a block when its $height\,mod\,1024 = 0$.
Parameters for the initial moment of time~$(height = 1)$ are hardcoded.

## Proposing a change and voting for it

To propose a change, in the first block of a voting epoch (of $1,024$ blocks, so in a block of
$height\,mod\,1024 = 0$), a miner is posting an identifier of a vote for a change. There are three slots (three bytes)
in a block header for proposed changes, with two slots reserved for everyday changes and the third one for
proposing a soft fork. A slot not occupied by a proposal is to be set to zero. Votes could come in any order.
Examples of the bytes: $(0, 1, 120)$, $(120, -3, 0)$. In the first case, a miner is proposing to increase the storage fee factor ($id:1$), and
also proposes a soft-fork ($id:120$); in the second case, a miner is proposing to decrease block size ($id:-3$), and also
 is proposing a soft-fork ($id:120$).

To vote for a proposal~(which is proposed in the first block of an epoch) within the epoch, a miner includes the vote identifier into the block header. Identifiers not proposed in the first block of the epoch are ignored.

If a majority of votes within an epoch support an everyday change (so at least 513 blocks contain an identifier), a new value of the parameter should be written into the extension section of the first block of the next epoch.

## Voting for a soft-fork

A soft-fork happens when a protocol version supported by the network is being increased.
The protocol version is being written into every block header, with the initial value during launch to be set to 1.

The semantics behind versioning is not defined ahead of time by the protocol and so up to clients and their developers.
Protocol developers can disable some existing validation rules from the [Validation](#validation) section during a soft-fork while introducing new ones.

The protocol version upgrade is to be done in the following steps:

- A protocol developer implements and releases software with changed rules and this software may deactivate some existing rules while also introducing new logic.
- A miner proposes increasing the protocol version and putting deactivated rules into extension.
- Other miners are voting within 32 epochs for the proposal
- If the soft-fork proposal is being rejected~(so if it gathers no more than $90\%$ of votes during the voting period, i.e. no more than $\lfloor 32 * 1024 * 90 / 100 \rfloor = 29491$ votes), new voting may be proposed next epoch after the voting is done.
- If the soft-fork proposal is approved, an activation period of 32 epochs is starting. The first block
after the activation period is called activation height. It is prohibited to vote for a new soft fork during the activation and the activation height. Soft-fork data is still to be written to corresponding extension sections~(see below) during the activation period and on activation height.
Block version written into extensions is to be increased from the first block of the activation period, while the protocol version in headers is still the same. The protocol version in headers is increased from the activation height.

To start voting for a soft fork, a miner needs to publish the identifier $120$ in the first block of the epoch; consider, for example, that its height is $h_s$. Next epoch, a miner should post height when the start fork was proposed ($122: h_s$) in the extension section of the block, and the number of votes collected in the previous epochs $v_s$ should be written there as well as ($121: v_s$).

See this [ergoforum post](https://www.ergoforum.org/t/voting-for-a-soft-fork-in-ergo/2958) for an example. 

### Examples:

- Assume that a vote for soft-fork is proposed in block number $1024$ (by writing a record into the extension with a key equal to $120$ and any value). Assume that within this epoch, before block number $2048$, $500$ votes were collected. A miner who generates block $\#2048$ must write the height when the soft-fork voting has been started in the extension section of the block as ($122: 1024$ key-value pair), as well as the number of votes supporting the fork gathered within the epoch done (in the form of $121: 500$). Assume that the new epoch started with the block $\#2048$ brings 600 votes for the fork. Then a miner generating the block $\#3072$ must write down the following pairs: $(121, 1100)$ and $(122, 1024)$.
- The voting is to be done on height $1024 + 1024*32 = 33792$, with the last vote written into block $\#33791$. Block $\#33792$ still should contain correct values for votes collected and voting starting height.
- let us assume that voting for the soft-fork was not successful, i.e. no more than $29491$ votes for soft-fork have been gathered between blocks $\#1024$~(inclusive) and $\#33792$~(exclusive). Then the next epoch block, the block $\#34816$ should clear the old voting parameter values. New voting for soft-fork may be started in this new epoch, so in the block $\#34816$, if the block contains a vote for the soft-fork (i.e. a record with key = 120 in the extension section), then the block must contain new starting height and votes collected values (i.e. following pairs: $(121: 0)$ and $(122: 34816)$). If there is no new voting started, all the parameters regarding soft-fork voting must be cleared off of the block $\#34816$.
- Now, assume that the voting for the soft-fork was successful, i.e. more than $29491$ votes for soft-fork have been gathered between blocks $\#1024$~(inclusive) and $\#33792$~(exclusive). In this case, the activation epoch is starting immediately after the voting has been done, so on height $33792$. The activation epoch lasts for 32 epochs, so the first block after the activation period has a height of $33792$. Please note that any vote for a soft-fork during the activation period is prohibited. Also, on the first block of a voting epoch, soft-fork voting parameters should be written~(height when voting had been started and also the number of votes collected). On the first block after activation, the protocol version written into a block must be increased. The first block after activation should carry soft-fork voting parameters. The parameters must be cleared next epoch so in a block $\#33792$. New voting may be started in the block $\#33792$, similarly to the case of a non-successful vote.


# Storage Rent

__We've designed Ergo with long-term economic sustainability in mind, and storage rent is one of the ways we're ensuring miners stay profitable well into the future. This can be thought of as 'on-chain garbage collection' that reduces the problem of blockchain bloat – and even makes it profitable.__

**Key Points**

- An important consequence of storage fees is that they provide additional rewards (besides block and transaction rewards) for miners.
- Storage fees decrease the storage load and eliminate extra costs that could be added during unreasonable state growth.
- Storage fees encourage coin flow and prevent deflation, which can cause illiquidity and the congestion of a currency system.

The 2020 block reward reduction was the most important halving event Bitcoin has experienced. This was the point where the narrative of programmatic scarcity and digital gold was truly be proven in the context of the sharpest economic downturn in living memory. In previous halvings, Bitcoin has still been in its infancy, a niche experiment. Future halvings will confirm the principle. But this one is the watershed.

Looking ahead, though, what happens in 20 or 30 years, when block rewards have fallen so far that miners have to rely on transaction fees and potentially other sources of revenue? Will Bitcoin be sustainable? What will be the impact on the ecosystem?

*The simple answer is that we don't know.*

Mining rewards are a key feature in maintaining the security of proof-of-work blockchains like Bitcoin and Ergo. And so, while we have deliberately kept many of Bitcoin's tried and tested features, we have updated this one to give miners a boost when block rewards have fallen to zero.

- [Ergo Explainer: Storage Rent](https://ergoplatform.org/en/blog/2022-02-18-ergo-explainer-storage-rent/)
- [Tracking storage rent potential](https://www.reddit.com/r/ergonauts/comments/tyymax/tracking_storage_rent_potential/)


## Storage fees

Fees will be deducted slowly, over time – the unmoved UTXOs will not simply be appropriated by miners. Anyone who wants to avoid this simply needs to move their balances once every four years, which is not an onerous requirement for helping incentivise miners and avoiding the deflationary consequences of lost coins. You can read more about how fees will be levied in [this paper](https://fc18.ifca.ai/bitcoin/papers/bitcoin18-final18.pdf).

In this way, Ergo seeks to ensure a balance between maintaining digital scarcity, on the one hand, and giving miners long-term incentives to secure the blockchain, on the other – long past the point where new coins have ceased to be released.


## Lost coins

Digital scarcity is an important feature of Ergo. Like Bitcoin, ERG is designed to be a finite resource and long-term store of value. We do not agree with the principle of infinite inflation.

And yet, this has to be balanced against the need to pay miners to secure the blockchain and process transactions. Without adequate compensation for miners, there is no viable blockchain at all. Ergo approaches this by slowly recycling lost coins, in a feature we call 'Storage rent'. 

Studies suggest that as many as [4 million BTC may have been lost forever](https://bitcoinist.com/estimated-4-million-bitcoin-lost-forever-by-users-forgetfulness/). These are coins that were mined in the early days of Bitcoin and stored on hard drives that were subsequently thrown away or destroyed because the owners forgot about them or thought they were worthless, as well as coins in addresses for which the private keys have been lost. (And, of course, there are Satoshi's estimated holdings of 1 million BTC, which may never move.)

Where coins have genuinely been permanently taken out of circulation in this way, it makes sense to have a mechanism to recover them and put them back into the blockchain economy. That way, we can preserve digital scarcity without unnecessarily accelerating it. In other words, by attempting to stick to the intended algorithmic supply for any given point in time.

Ergo's halving schedule is faster than Bitcoin's. Block rewards start at 75 ERG and decrease steadily after the first two years. There is no 'long tail' of emission, and after eight years, block rewards will fall to zero. After that, the total supply will be fixed. The number of ERG in existence will never be more than 97,739,925.


## A Systematic Approach To Cryptocurrency Fee

This article is a continuation and summarization of *[A Systematic Approach To Cryptocurrency Fees](https://fc18.ifca.ai/bitcoin/papers/bitcoin18-final18.pdf)* (hereinafter referred to as the paper) by Alex (Kushti) Chepurnoy, Vasily Kharin and Dmitry Meshkov. In the paper, the authors address the problem of storage resources utilization. There is a concern that once an element of the state is created, it exists forever and inevitably balloons node disk space. This will lead to unreasonable state growth of the blockchain.

While cryptocurrencies address transaction fees as an atomic concept, the paper suggests that it is reasonable to take this into account on a 3-dimensional scale.

![Figure A.](https://ergoplatform.org/img/uploads/3d.png)



### Blockchain Costs

Proof of Work blockchain technology relies on miners to guard the integrity of the blockchain. Miner resources, such as memory and electricity, are costly, and therefore a revenue scheme is needed to incentivize miners. Miner incentives are currently comprised of block rewards and transaction fees. Transactions fees are an important component in preventing spam attacks that exhaust miner resources.

Besides network utilization, transaction processing requires a miner to spend resources to maintain all the original blockchain data. In the case of Bitcoin, this might be less of a problem because it has yet to implement smart contract functionality. Cryptocurrencies that support smart contract languages, such as Solidity (Ethereum), however, may require a lot of computations, and corresponding costs will be included in the transaction fee.

The 3-dimensional scale shown above is based on storage-oriented load, computational load and network load.

* Storage-oriented load refers to the additional cost of storing old data in the blockchain. 
* Computational load is created by the execution of smart contracts. 
* Network load is all the transactions that do not exist in the current block but will be added to the next block.

In Ergo, the total size of the state is the sum of the sizes of all UTXOs. That is to say that this data contains the execution of smart contracts, all the transactions and nodal information. Because the memory resources provided by miners are limited, a state deterioration fee should be added to miners' revenue streams in order to encourage decreasing the system load while securing future miners' contributions.

### State Growth

**Unreasonable state growth** is an economic problem, and it can lead to spam attacks and network congestion. Another problem could be the deflation of a cryptocurrency if coins are lost and/or forgotten. So instead of being used as the base for smart contracts, the currency becomes unreasonably scarce, making the system heavy and limiting coin flow.

This leads to a perpetually increasing state (e.g. the Bitcoin's total UTXO size), and the state may grow faster during spam attacks. For example, 15 million outputs were created during spam attacks against Bitcoin in July 2015. An attack on Ethereum created 18 million new accounts added to the state - which previously held only 1 million - and performed successful "denial of service" attacks against the nodes.

To tackle the problem of unreasonable state growth, a "storage rent" fee is proposed by the paper. Storage rent is a scheduled fee that is based on the continuation of each UTXO created in the blockchain. This is achieved by the use of scheduled payments, which will eradicate the unused bytes after a certain time.

Additionally, the use of blockchains as cloud storage is gaining attraction, so permanently storing objects in the state without some form of recirculation procedure of the old data is not a plausible option.

For the purposes of research and this article, it is worth noting that the concept of storage rent was also proposed in 2014 by [Freicoin](http://freico.in):

> *"Demurrage forces freicoins to circulate at deliberately high rates. Separation of money's roles as store-of-value and medium-of-exchange allows money to flow when it is needed, in good times and bad. "*


## Resources

- [Storage rent details](https://www.ergoforum.org/t/storage-rent-details/256)
- [HF-4.0 Reduce storage rent period #1144](https://github.com/ergoplatform/ergo/issues/1144) - Rejected


# Log-Space Mining

Dionysis Zindros explains the technical landscape of Non-Interactive Proofs of Proof-of-Work. Dionysis takes a diligent approach for the Ergo Cast with a detailed rundown of what Non-Interactive Proofs of Proof-of-Work truly are. Furthermore, Dionysis evaluates the operation, implementation, and impact that his primitive delivers upon. 

- [NiPoPoWs & Log-Space Mining – Ergo Cast Episode #5](https://ergocast.io/episode/nipopows-ergo-cast-episode-5/)


This section is based on a [recently published](https://eprint.iacr.org/2021/623.pdf) article by IOHK. For an additional resource, please see the following [video.](https://www.youtube.com/watch?v=s05ypkSC7gk)

## Overview

Miners must constantly maintain the blockchain, whether it is Ergo, Bitcoin, or another PoW consensus model. In addition to using computational resources, miners also use storage resources that maintain all blockchain data from the genesis block.

A new miner's problem: Is downloading all the data from the genesis block strictly necessary? Why is it not possible to download only the most relevant blocks to maintain the network?

The block headers of the blockchain should be enough to access the necessary data. [NIPoPoWs](https://nipopows.com/) (Non-Interactive Proofs of Proof of Work) can be integrated to form interlinked block header sets that will reduce historical data storage.

When needing to access key blocks in the blockchain, miners should be able to do this from the headers of the old blocks efficiently. That is because each new block must indicate all of the current networks. As new blocks are created, a set of new block headers can be enough to check for the current UTXO set. Since the new blocks contain the data of old stringed block header sets, it enables light mining by eliminating the need to download all the blockchain data.

What are we trying to optimise by stringing old PoW history and compiling it into a snapshot?

If we say C=old blocks and K=new blocks, then included blocks in the snapshot can be growing when K=new blocks are constant, and C=old blocks are linear. But it can also be shrinking depending on the smart contract applications. The problem of maintaining heavy loads of data by the miners can be solved by bootstrapping through NIPoPoWs. 


## NIPoPoW Implementation

Instead of accessing all of the blocks, superblocks (or light-clients) are enough to verify all of the blocks. This is accomplished by maintaining the historical data of the blockchain through smart contracts. The introduction of these superblock clients on NIPoPoWs can be done via 'velvet' or soft forks, and after that "light" miners can bootstrap through "online" mining.

NIPoPoWs enable smart contracts to maintain historical data so that new "light" miners can work in a so-called "online" fashion. This is the main idea of Logarithmic Space Mining. Instead of saving all the blockchain data locally on nodes, the unnecessary part can be compiled into the blockchain itself. New miners do not need to carry the historical data, and as they continue to mine, new "light" miners will help other "light" miners bootstrap. There will be no need to carry old historical data, and old miners can abandon historical data for lighter mining. This is how the whole miner population can abandon old blocks and make the system much more efficient.
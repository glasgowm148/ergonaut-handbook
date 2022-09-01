---
title: Storage Rent
description: 
published: true
date: 2022-09-01T21:32:44.213Z
tags: 
editor: markdown
dateCreated: 2021-03-02T19:06:27.106Z
---

# Storage Rent
**tl;dr: Storage Rent is a fee for long term storage on the Ergo blockchain. You will be charged ~0.14 ERG and a transaction fee for any box (UTXO) of yours that remains dormant (unspent) for 4 years, to pay for the costs of storing your digital information. You can avoid this fee by periodically "consolodating your boxes".**  

We've designed Ergo with long-term economic sustainability in mind, and storage rent is one of the ways we're ensuring miners stay profitable well into the future. This can be thought of as 'on-chain garbage collection' that reduces the problem of blockchain bloat – and even makes it profitable.

**Key Points**

- An important consequence of Storage Rent fees is that they provide additional rewards (besides block and transaction rewards) for miners.
- Storage fees decrease the network's storage load and eliminate extra costs that could be added during unreasonable state growth.
- Storage fees encourage coin flow and prevent deflation, which can cause illiquidity and the congestion of a currency system.

**Bitcoin without the Block Reward**

The 2020 block reward reduction will probably be the most important halving Bitcoin ever experiences. This is the point where the narrative of programmatic scarcity and digital gold will truly be proven, in the context of the sharpest economic downturn in living memory. In previous halvings, Bitcoin has still been in its infancy, a niche experiment. Future halvings will confirm the principle. But this one is the watershed.

Looking ahead, though, what happens in 20 or 30 years, when block rewards have fallen so far that miners have to rely on tx fees and potentially other sources of revenue? Will Bitcoin be sustainable? What will be the impact on the ecosystem?

The simple answer is that we don’t know.

Mining rewards are a key feature in maintaining the security of proof-of-work blockchains like Bitcoin and Ergo. And so, while we have deliberately kept many of Bitcoin’s tried and tested features, we have updated this one to give miners a boost when block rewards have fallen to zero.

**Lost coins**

Digital scarcity is an important feature of Ergo. Like Bitcoin, ERG are designed to be a finite resource and long-term store of value. We do not agree with the principle of infinite inflation.

And yet, this has to be balanced against the needs to pay miners to secure the blockchain and process transactions. Without adequate compensation for miners, there is no viable blockchain at all. Ergo approaches this by slowly recycling lost coins, in a feature we call ‘Storage Rent’.

Studies suggest that as many as [4 million BTC may have been lost forever](https://bitcoinist.com/estimated-4-million-bitcoin-lost-forever-by-users-forgetfulness/). These are coins that were mined in the early days of Bitcoin and stored on hard drives that were subsequently thrown away or destroyed because the owners forgot about them or thought they were worthless, as well as coins in addresses for which the private keys have been lost. (And, of course, there’s Satoshi’s estimated holdings of 1 million BTC, which may never move.)

Where coins have genuinely been permanently taken out of circulation in this way, it makes sense to have a mechanism to recover them and put them back into the blockchain economy. That way, we can preserve digital scarcity without unnecessarily accelerating it. In other words, by attempting to stick to the intended algorithmic supply for any given point in time.
 


Ergo’s halving schedule is faster than Bitcoin’s. Block rewards start at 75 ERG, and decrease steadily after the first two years. ~~There is no ‘long tail’ of emission, and after eight years block rewards will fall to zero.~~ The number of ERG in existence will never be more than 97,739,925.

> NOTE: EIP-27 is extending Ergo's original 8 year emission schedule via soft-fork. After passing (with over 90% of miners voting in favor), the proposal to "retarget" emissions was activated on mainnet with block 777,217 (June 21, 2022). **Although Ergo's emission schedule has been extended, the max supply of ERG is stictly preserved and will never change.**
</br>
Anyone interested can review the final proposal on the [EIP-27 GitHub page](https://github.com/ergoplatform/eips/blob/master/eip-0027.md), join the previous community discussion on
[Ergo Emission: details, retargeting via a soft-fork](https://www.ergoforum.org/t/ergo-emission-details-retargeting-via-a-soft-fork/2778/21), and read this [blog post](https://ergoplatform.org/en/blog/A-New-Era-for-Ergo-EIP-27-Begins-Today/) for further details about the updated emissions schedule. 
{.is-warning}


**Storage fees**

From that point, however, miners will need further incentives to secure the network. Miners have ongoing costs in terms of bandwidth and storage, and in cases where coins are simply left for years, there is typically no charge for reflecting the value of securing them. The tx fee that is paid up-front in Bitcoin is the only charge ever made for storing those coins.

In Ergo, in addition to transaction fees, miners will also be able to collect Storage Rent fees on UTXOs that have not been moved for four years or more.

Fees will be deducted slowly, over time – the unmoved UTXOs will not simply be appropriated by miners. Anyone who wants to avoid this simply needs to move their balances once every four years, which is not an onerous requirement for helping incentivise miners and avoiding the deflationary consequences of lost coins. You can read more about how fees will be levied in [this paper](https://fc18.ifca.ai/bitcoin/papers/bitcoin18-final18.pdf).

In this way, Ergo seeks to ensure a balance between maintaining digital scarcity, on the one hand, and giving miners long-term incentives to secure the blockchain, on the other – long past the point where new coins have ceased to be released.

**Welcome to Smart Money**

[Facebook](http://www.facebook.com/sharer.php?u=https%3a%2f%2fergoplatform.org%2fen%2fblog%2f2020_02_12_welcome_to_smart_money%2f)

[Twitter](https://twitter.com/share?url=https%3a%2f%2fergoplatform.org%2fen%2fblog%2f2020_02_12_welcome_to_smart_money%2f&hashtags=ergoplatform)

[Ergoplatform.org](https://ergoplatform.org/en/blog/2020_02_12_welcome_to_smart_money/)
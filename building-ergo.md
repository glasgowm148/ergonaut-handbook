---
title: Building Ergo
description: 
published: true
date: 2021-03-02T19:06:27.106Z
tags: 
editor: markdown
dateCreated: 2021-03-02T19:06:27.106Z
---

# Oracles

**Blockchains are siloed systems that can only reference their own data, established by consensus. Oracles are the solution to the problem of working with external information, which is vital for many everyday use cases.**

Blockchains are intentionally self-contained. They reference information only recorded within their immediate ecosystem, that has been agreed upon by a majority of miners. Since the whole point of a blockchain, based on consensus, is that there are no sources of centralisation or single points of failure, that poses a problem.

What happens when you want to engage with external information? Many blockchain-based applications need to process data from the real world. That might be financial information, such as market data and prices from exchanges, for DeFi applications; it could be sporting results, for eSports predictions markets; it could even be [atmospheric noise information, for random number generators](https://www.random.org/).

**Introducing Oracles**

Oracles are the software that serves as a link between these real-world sources of data and the siloed world of the blockchain. They are simple in principle, since they only need to create a series of transactions with the necessary data (ideally formatted in an easily-accessible way) at regular intervals.

However, while anyone can record information to an open blockchain, that is a source of centralisation. So how do you trust an oracle?

The answer is: you don’t. Just like the blockchain’s consensus method itself, you need multiple oracles pulling data from multiple sources, then coming to agreement about the value to record to the blockchain. So you don’t need to trust an individual miner, and you don’t need to trust an individual oracle.

**Example: bitcoin price data**

As an example, let’s say we want to record bitcoin’s closing price every day to the Ergo blockchain, to give us a long-term and reliable source of price data.

We could take a dozen – or even a hundred – different data feeds, each pulling data from a major exchange. Coinbase, Bitstamp, Kraken, and so on. We make sure that many exchanges are represented, and while it’s good to have several examples of data from the same exchange, we don’t want any exchange over-represented.

Then the parties need to reach consensus about the price. Let’s say there are 100 parties and prices involved. There are different ways they could do that:

* Take the mean of all the prices they provide
* Discard the highest and lowest 20 prices, and take the mean of the remaining 60 prices
* Select the median price
* Weight the prices, with the central cluster of prices having greater weight, and take the mean

The aim is to discard or downweight any outliers, which could be due to extreme price fluctuations on a single exchange, API outages, or dishonest oracle data providers, while retaining many good data points to ensure a single reliable record of price.

Oracles are a hugely important part of the blockchain ecosystem. Once you have robust oracles in place, you can create all kinds of DeFi applications – including stablecoins, which are a vital part of the blockchain economy, and one we’ll be exploring on Ergo in the coming months.

# Atomic Swaps

**Blockchains are siloed systems that can only reference their own data, established by consensus. Oracles are the solution to the problem of working with external information, which is vital for many everyday use cases.**

Blockchains are intentionally self-contained. They reference information only recorded within their immediate ecosystem, that has been agreed upon by a majority of miners. Since the whole point of a blockchain, based on consensus, is that there are no sources of centralisation or single points of failure, that poses a problem.

What happens when you want to engage with external information? Many blockchain-based applications need to process data from the real world. That might be financial information, such as market data and prices from exchanges, for DeFi applications; it could be sporting results, for eSports predictions markets; it could even be [atmospheric noise information, for random number generators](https://www.random.org/).

**Introducing Oracles**

Oracles are the software that serves as a link between these real-world sources of data and the siloed world of the blockchain. They are simple in principle, since they only need to create a series of transactions with the necessary data (ideally formatted in an easily-accessible way) at regular intervals.

However, while anyone can record information to an open blockchain, that is a source of centralisation. So how do you trust an oracle?

The answer is: you don’t. Just like the blockchain’s consensus method itself, you need multiple oracles pulling data from multiple sources, then coming to agreement about the value to record to the blockchain. So you don’t need to trust an individual miner, and you don’t need to trust an individual oracle.

**Example: bitcoin price data**

As an example, let’s say we want to record bitcoin’s closing price every day to the Ergo blockchain, to give us a long-term and reliable source of price data.

We could take a dozen – or even a hundred – different data feeds, each pulling data from a major exchange. Coinbase, Bitstamp, Kraken, and so on. We make sure that many exchanges are represented, and while it’s good to have several examples of data from the same exchange, we don’t want any exchange over-represented.

Then the parties need to reach consensus about the price. Let’s say there are 100 parties and prices involved. There are different ways they could do that:

* Take the mean of all the prices they provide
* Discard the highest and lowest 20 prices, and take the mean of the remaining 60 prices
* Select the median price
* Weight the prices, with the central cluster of prices having greater weight, and take the mean

The aim is to discard or downweight any outliers, which could be due to extreme price fluctuations on a single exchange, API outages, or dishonest oracle data providers, while retaining many good data points to ensure a single reliable record of price.

Oracles are a hugely important part of the blockchain ecosystem. Once you have robust oracles in place, you can create all kinds of DeFi applications – including stablecoins, which are a vital part of the blockchain economy, and one we’ll be exploring on Ergo in the coming months.


# Storage Rent

**We’ve designed Ergo with long-term economic sustainability in mind, and storage rent is one of the ways we’re ensuring miners stay profitable well into the future. One community member, Robert, describes this function as ‘on-chain garbage collection’ that reduces the problem of blockchain bloat – and even makes it profitable.**

The 2020 block reward reduction will probably be the most important halving Bitcoin ever experiences. This is the point where the narrative of programmatic scarcity and digital gold will truly be proven, in the context of the sharpest economic downturn in living memory. In previous halvings, Bitcoin has still been in its infancy, a niche experiment. Future halvings will confirm the principle. But this one is the watershed.

Looking ahead, though, what happens in 20 or 30 years, when block rewards have fallen so far that miners have to rely on tx fees and potentially other sources of revenue? Will Bitcoin be sustainable? What will be the impact on the ecosystem?

The simple answer is that we don’t know.

Mining rewards are a key feature in maintaining the security of proof-of-work blockchains like Bitcoin and Ergo. And so, while we have deliberately kept many of Bitcoin’s tried and tested features, we have updated this one to give miners a boost when block rewards have fallen to zero.

**Lost coins**

Digital scarcity is an important feature of Ergo. Like Bitcoin, ERG are designed to be a finite resource and long-term store of value. We do not agree with the principle of infinite inflation.

And yet, this has to be balanced against the needs to pay miners to secure the blockchain and process transactions. Without adequate compensation for miners, there is no viable blockchain at all. Ergo approaches this by slowly recycling lost coins, in a feature we call ‘Storage rent’.

Studies suggest that as many as [4 million BTC may have been lost forever](https://bitcoinist.com/estimated-4-million-bitcoin-lost-forever-by-users-forgetfulness/). These are coins that were mined in the early days of Bitcoin and stored on hard drives that were subsequently thrown away or destroyed because the owners forgot about them or thought they were worthless, as well as coins in addresses for which the private keys have been lost. (And, of course, there’s Satoshi’s estimated holdings of 1 million BTC, which may never move.)

Where coins have genuinely been permanently taken out of circulation in this way, it makes sense to have a mechanism to recover them and put them back into the blockchain economy. That way, we can preserve digital scarcity without unnecessarily accelerating it. In other words, by attempting to stick to the intended algorithmic supply for any given point in time.

Ergo’s halving schedule is faster than Bitcoin’s. Block rewards start at 75 ERG, and decrease steadily after the first two years. There is no ‘long tail’ of emission, and after eight years block rewards will fall to zero. After that, total supply will be fixed. The number of ERG in existence will never be more than 97,739,925.

**Storage fees**

From that point, however, miners will need further incentives to secure the network. Miners have ongoing costs in terms of bandwidth and storage, and in cases where coins are simply left for years, there is typically no charge for reflecting the value of securing them. The tx fee that is paid up-front in Bitcoin is the only charge ever made for storing those coins.

In Ergo, in addition to transaction fees, miners will also be able to collect storage rent fees on UTXOs that have not been moved for four years or more.

Fees will be deducted slowly, over time – the unmoved UTXOs will not simply be appropriated by miners. Anyone who wants to avoid this simply needs to move their balances once every four years, which is not an onerous requirement for helping incentivise miners and avoiding the deflationary consequences of lost coins. You can read more about how fees will be levied in [this paper](https://fc18.ifca.ai/bitcoin/papers/bitcoin18-final18.pdf).

In this way, Ergo seeks to ensure a balance between maintaining digital scarcity, on the one hand, and giving miners long-term incentives to secure the blockchain, on the other – long past the point where new coins have ceased to be released.

Share post:

[Facebook](http://www.facebook.com/sharer.php?u=https%3a%2f%2fergoplatform.org%2fen%2fblog%2f2020_02_12_welcome_to_smart_money%2f)

[Twitter](https://twitter.com/share?url=https%3a%2f%2fergoplatform.org%2fen%2fblog%2f2020_02_12_welcome_to_smart_money%2f&hashtags=ergoplatform)

[Ergoplatform.org](https://ergoplatform.org/en/blog/2020_02_12_welcome_to_smart_money/)
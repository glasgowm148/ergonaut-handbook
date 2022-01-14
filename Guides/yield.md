---
title: Yield
description: Earn Yield with your ERG
published: true
date: 2022-01-14T04:27:56.144Z
tags: 
editor: markdown
dateCreated: 2021-12-30T10:43:30.389Z
---

# Earning Yield

Ergo is a **Proof of Work** blockchain. So, it is not possible to stake Ergo itself as you would in a **Proof of Stake** blockchain. However, it is possible to 'stake' native tokens on Ergo, either in combination with Ergo in liquidity pools, tokenisation of dApps, trading bots. lending platforms and other mechanisms. 

## ErgoProfitSharingDapp

- [GitHub](https://github.com/mhssamadani/ErgoProfitSharingDapp)

This service will provide a way for dapps to distribute gains among dapps' token holders.

The first implementation of this will tokenise Ergomixer. (Auction House and Raffle thereafter)

The ErgoMixer income (in ERG and other tokens) is currently received by its creator ('anon2020s'), since it has only one stakeholder at the moment. He has announced that he is willing to create and sell some tokens in the near future to obtain more stakeholders; let's call this token $MIX. Later, anyone with these $MIX tokens can stake them in the Profit Sharing contract and obtain the mixer's incomes proportional to their staked tokens.

So, it will not be way a way to 'stake' ERG at first. However in the future it could be used in some creative services to provide ERG-staking.

More details available on the [ergoforum](https://www.ergoforum.org/t/a-solution-for-staking/1057)

## Staking

Several other projects plan to launch native tokens on Erg and plan to offer staking.

- [ErgoPad](https://ergopad.io/staking)
- [anetaBTC](https://www.reddit.com/r/anetaBTC/)
- [ERGnomes.io](https://ergnomes.io)

# AMMs

An Automated Market Maker (AMM) uses mathematical models to set the price and match buyers and sellers rather than merely matching buy and sell orders, as in traditional order-books. AMM is best in markets with low liquidity. 

One of the features of AMM is that liquidity providers add assets to the exchange for a fee, and the market benefits from an increase in liquidity, smaller latency, limited price slippage, and less market volatility when using this additional liquidity.

## Impermanent Loss / Volitality Harvesting

Impermanent loss (IL) occurs when the mathematical formula of an AMM adjusts the asset ratio in a pool to ensure both assets remain at an even value. 

Example: You enter an AMM pool of Erg/SigUSD, when the prices of each of these assets is at $10 and $1. So, you put in 1 Erg for every $10 SigUSD into the pool. 

Then, Erg's price goes to $20 a month later. Let's assume you earned $2 in fees. You'll then have 0.8 Erg and $16 SigUSD to have even amounts in the pool, or $32. The higher the price of Erg relative to SigUSD, the less Erg you have.

So, why would anyone provide liquidity to an AMM in an asset they expected to go up and a stablecoin like SigUSD? The answer: volitality harvesting.

There's an [involved paper](https://research.paradigm.xyz/uniswaps-alchemy), but here's the central idea: digital assets like Erg don't just increase. They have a lot of volitality, ups and downs, and if you are in an AMM liquidity pool, the balancing of the AMM of the pool works as a kind of dollar cost averaging. It buys more of the asset that costs less when it is down and less of the asset that costs more when it is up.

## ErgoDex

![screenshot_2022-01-09_at_18.13.43.png](/screenshot_2022-01-09_at_18.13.43.png)
There is currently one decentralized exchange on Ergo, Ergodex. There are several pools on ErgoDex with a visible estimated asset annual percentage yield (APY) that can be used for yield harvesting.

Your redeemable amount changes as the pool gets used and a percentage of the swaps are earned by the pool. You get a percent of the pool fee proportional to your stake.

- SigRSV/ERG pair
	-	Minimises impermanent loss (both coins move in the same direction price-wise)
- SigUSD/ERG
	- High IL risk, however a solid investment if you want to earn fee's off your nest-egg. SigUSD has has never came close to loosing it's peg. 

**Community Chats**
- [SigmaUSD Telegram](https://t.me/SigmaUSD)
- [ErgoDex Telegram](https://t.me/ergodex_community)

### Swop.fi

- AMM Pool

## Centralised Exchanges
While not without risk, several options are available to earn some returns on your ERG. 


### CoinEx

There is an AMM Pool available on CoinEx. Please be aware of impermanent loss. 



# Trade Bots 



## KuCoin

KuCoin offers perhaps the most simple ways to earn yield on your Erg with it's infinity grid bot. It has the following bots available.


- Infinity Grid
- Spot Grid
- Futures Grid
- DCA Bot

The **Spot grid** bot trades with a grid, selling high and buying low. The problem is that if ERG goes way above your range, you will have sold all your ERG and be left holding USDT. (Impermanent loss)

The **Infinity Grid** bot works like the spot grid, but has no set range, and your bids with the price. 

The **Futures Grid** bot is still unfortunately unavailable for ERG. 

The **DCA bot** reduces the risk of purchasing high by investing at consistent intervals.

- [ERG: Technical Analysis & Botting Telegram](https://t.me/ERGTechnicalAnalysis)


## Others
Rather than using the bots on KuCoin, you can use custom bots with a bit more control over your trading strategy. 

- 3commas
- shrimpy.io

# Index Funds

## ergo-index

[ergo-index.fund](https://ergo-index.fund) is a non-custodial platform that enables users to pool their funds together to invest in a portfolio of tokens on the Ergo blockchain. (still in development / not operational. )


- [GitHub](https://github.com/ergo-index)


# Lending

## ErgoLend

- [ergolend.org](https://www.ergolend.org/#)

## Liqwid

Requires ERG as a native ADA token. 

- [Liqwid.io Tweet](https://twitter.com/liqwidfinance/status/1412600854008537089)

## Gate.io

You can lend there for around 3.5%


# Trading


### Gate.io

Offers leveraged trading. 

## Technical Analysis
- [ERG: Technical Analysis & Botting Telegram](https://t.me/ERGTechnicalAnalysis)
- [Alternative to TradingView](https://www.livecoinwatch.com/price/Ergo-ERG)
- [Bitcoin Stats](https://www.lopp.net/bitcoin-information/statistics-metrics.html)
- [Chainanalysis](https://markets.chainalysis.com)
- [The Pattern Site](http://thepatternsite.com/barrb.html)



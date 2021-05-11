---
title: SigmaUSD
description: 
published: true
date: 2021-05-11T13:22:18.269Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:02:25.004Z
---

> Introducing [SigmaUSD.io](https://sigmausd.io/#/) the first UTxO-based stable coin - an instantiation of the [AgeUSD protocol](https://github.com/Emurgo/age-usd). The foundation on which a new era of digital finance will be built.
>
>Its economic model designed in partnership between IOHK, Ergo, and Emurgo maintains the conservative settings for collateral reserves and avoids the need for liquidations. Along with that, it supports a fully decentralised stablecoin emission setup. **Thus, SigmaUSD will offer the world a stable, simple, and decentralised stablecoin.**
{.is-success}


- [SigmaUSD vs the competition.](https://curiaregiscrypto.medium.com/sigmausd-vs-the-competition-e70b23fe37a3)
- [SigmaUSD on Ergo - Privacy, Stability and Governance](https://curiaregiscrypto.medium.com/sigmausd-on-ergo-a36e0cdff743)
- [Building Ergo: How the AgeUSD stablecoin works](https://ergoplatform.org/en/blog/2021-02-05-building-ergo-how-the-ageusd-stablecoin-works/)

# Overview


**Assuming Erg is $1;**

- You take 100 ERG worth $1 each and mint them into either StableCoins or ReserveCoins
- If you mint SigmaRSV, and the price goes up 10% — you get back 110 ERG when you cash out.
- If you mint into the SigmaUSD, and the price goes up 10% — you still get $100 out, but because its went up 10%, you get 90ERG

> This is the simplest example possible to explain how the logic of the contract works (without fees) and not what happens in real world scenario. The value you can redeem for your SigRSV floats up and down based on transaction fees and profits/losses SigUSD holders take when withdrawing.
{.is-warning}


**The 2% fee taken during minting goes back into the reserve**
- This fee accumulates in the reserve.
- SigmaRSV is an **option call on the reserve**. 
- When price dips, SigUSD holders who exit at a lower point than they entered, they must be rewarded extra erg to make their SigUSD up to $1
- SigRSV profits depend on these accumulated transaction fees minus any withdrawn by SigUSD holders. 



> This provides individuals with the ability to choose to either go **long** on Erg by minting **SigmaRSV** or to choose **stability** by minting **SigmaUSD.**
{.is-info}





## Advantages over MakerDAO
> **No liquidations!**
{.is-success}

Unlike Ethereum-based crypto-backed stablecoins, such as DAI, Emurgo introduces a Staticoin protocol-inspired design that does not rely on CDPs (Collateralized Debt Positions). The reason for this is the vulnerability of CDP-based protocols in terms of high volatility and blockchain congestion. As Emurgo states, "Black Thursday," when MakerDAO CDPs were triggered for liquidation due to volatility and then sold for $0 due to blockchain congestion that prevented others from bidding, demonstrated that a new design is needed. For SigmaUSD, this scenario is not possible.


**See these other articles for more information**
- [FAQ](/SigmaUSD/FAQ)
- [Detailed Overview](/SigmaUSD/Overview)


# SigmaUSD v1


- [Finding The Right Balance](https://ergoplatform.org/en/blog/2021_03_04-finding-right-balance/)
- [Community Discussion on Reddit](https://www.reddit.com/r/ergonauts/comments/lx7an4/sigmausd_dao_bank_is_a_complex_beast_highlevel/gpr96fq/?context=3)



# Resources

- SigmaUSD is an instantiation of AgeUSD which was inspired by [StatiCoin](http://staticoin.com/whitepaper.pdf)
- You can now mix your SigUSD and SigRSV coins directly into the [ErgoMixer](/ErgoMixer)

## Articles
- You can read the official [Emurgo announcement blog post here](https://ergoplatform.org/en/blog/2021_02_26-sigmausd-released/)
- https://thedailychain.com/hoskinson-cardano-working-on-stablecoin-to-rival-makerdao-developing-defi-products/
- [Erg/USD Explorer](https://explorer.ergoplatform.com/en/oracle-pool-state/ergusd) 
- [Ergo Summit 2021 - The IOHK Perspective - Designing the AgeUSD StableCoin](https://youtu.be/zG-rxMCDIa0?t=9247)


## Infographics

![screenshot_2021-02-25_at_19.14.01.png](/screenshot_2021-02-25_at_19.14.01.png)

---
title: SigmaUSD
description: 
published: true
date: 2021-03-04T19:09:47.345Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:02:25.004Z
---

> Introducing [SigmaUSD.io](https://sigmausd.io/#/) the first UTxO-based stable coin - an instantiation of the [AgeUSD protocol](https://github.com/Emurgo/age-usd). The foundation on which a new era of digital finance will be built.
>
>Its economic model designed in partnership between IOHK, Ergo, and Emurgo maintains the conservative settings for collateral reserves and avoids the need for liquidations. Along with that, it supports a fully decentralised stablecoin emission setup. **Thus, SigmaUSD will offer the world a stable, simple, and decentralised stablecoin.**
{.is-success}

# Overview 
IOHK, Ergo, and Emurgo designed the economic model of SigmaUSD. Its economic model maintains the conservative settings for collateral reserves and avoids the need for liquidations. Along with that, it supports a fully decentralised stablecoin emission setup. Thus, SigmaUSD will offer the world a stable, simple, and decentralised stablecoin.

**Reserve Providers** submit Ergs to the dApp's reserves and by doing so mint ReserveCoins (**SigmaRSV**). Each SigmaRSV represent a portion of the underlying Erg reserves held in the dApp.

**SigmaUSD** Users also submit Ergs to the dApp reserves; however, in their case, they mint SigmaUSD instead. This is only allowed by the protocol if there are sufficient reserves within the dApp (reserves are above the minimum reserve ratio). At any given moment, a SigmaUSD user can redeem their SigmaUSD in exchange for an amount of Ergs from the reserves equal to the current exchange rate as sourced by the Erg-USD [oracle pool](https://explorer.ergoplatform.com/en/oracle-pool-state/ergusd). 

Reserve Providers can only redeem their ReserveCoins for Ergs if the price of Ergs goes up (or a substantial amount of protocol fees are collected) and thus cover the value of all existing minted SigmaUSD plus an extra margin. By redeeming their ReserveCoins, they profit as they receive more underlying reserve cryptocurrency than when they minted their ReserveCoins (the increased amount coming from users who minted SigmaUSD).

> Reserve Providers allow SigmaUSD users to enjoy the stability of value. On their end, the Reserve Providers absorb the potential upside (if the value of the reserves goes up via the price of Ergs increasing compared to USD) and absorb the potential downside (if the underlying cryptocurrency in reserve goes down in price).
{.is-info}


# Basic overview

**Assuming Erg is $1;**

- You take 100 ERG worth $1 each and mint them into either StableCoins or ReserveCoins
- If you mint SigmaRSV, and the price goes up 10% — you get back 110 ERG when you cash out.
- If you mint into the SigmaUSD, and the price goes up 10% — you still get $100 out, but because its went up 10%, you get 90ERG

> This provides individuals with the ability to choose to either go **long** on Erg by minting **SigmaRSV** or to choose **stability** by minting **SigmaUSD.**
{.is-info}

**The 1% fee goes back into the reserve**
- This fee accumulates in the reserve.
- SigmaRSV is an option call on the reserve. (You own a %)
- When price dips, SigUSD holders who exit at a lower point than they entered, they must be rewarded extra erg to make their SigUSD up to $1
- SigRSV profits depend on these accumulated transaction fees minus any withdrawn by SigUSD holders. 

- [FAQ](/SigmaUSD/FAQ)
- 



## Advantages over MakerDAO
> **No liquidations!**
{.is-success}

Unlike Ethereum-based crypto-backed stablecoins, such as DAI, Emurgo introduces a Staticoin protocol-inspired design that does not rely on CDPs (Collateralized Debt Positions). The reason for this is the vulnerability of CDP-based protocols in terms of high volatility and blockchain congestion. As Emurgo states, "Black Thursday," when MakerDAO CDPs were triggered for liquidation due to volatility and then sold for $0 due to blockchain congestion that prevented others from bidding, demonstrated that a new design is needed. For SigmaUSD, this scenario is not possible.

As the community is going straight to the SigmaUSD-based stablecoin launch, we recommend again this impressive presentation by Bruno Woltzenlogel Paleo, "An IOHK Perspective: Designing The SigmaUSD Stablecoin Protocol — An Economic Analysis" from the ErgoSummit.





# Issues

## Failed transactions
There is currently significant demand. With Ergo being in the UTXO model and all of the dApp design patterns being quite young, we have limitations for the throughput. We have many high-level design ideas to address this for the future, with asynchronous EUTXO protocols, but this is still being deeply researched. 

We decided that it was better for the community to have something in the near term rather than waiting another year for the research to solidify into an implementation.


## Lower than expected profits

SigRSV is a **long** position, shorters were able to use their volume to profit off the dips during the initial launch. Their ability to do so has been reduced now so transactions will be building up at a faster rate. 

[SigmaUSD DAO bank is a complex beast - ergoforums.org](https://www.ergoforum.org/t/sigmausd-dao-bank-is-a-complex-beast/767)

# Resources

## StatiCoin

SigmaUSD is an instantiation of AgeUSD which was inspired by [StatiCoin](http://staticoin.com/whitepaper.pdf)

## ErgoMixer

You can now mix your SigUSD and SigRSV coins directly into the [ErgoMixer](/ErgoMixer)

## Articles
- You can read the official [Emurgo announcement blog post here](https://ergoplatform.org/en/blog/2021_02_26-sigmausd-released/)
- https://thedailychain.com/hoskinson-cardano-working-on-stablecoin-to-rival-makerdao-developing-defi-products/
- [Erg/USD Explorer](https://explorer.ergoplatform.com/en/oracle-pool-state/ergusd) 
- [Ergo Summit 2021 - The IOHK Perspective - Designing the AgeUSD StableCoin](https://youtu.be/zG-rxMCDIa0?t=9247)


## Infographics

![screenshot_2021-02-25_at_19.14.01.png](/screenshot_2021-02-25_at_19.14.01.png)
![unknown.png](/unknown.png)
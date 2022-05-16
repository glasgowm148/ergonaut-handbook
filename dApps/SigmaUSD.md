---
title: dApps/SigmaUSD
description: 
published: true
date: 2022-05-16T15:07:46.127Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:02:25.004Z
---

> Introducing [SigmaUSD.io](https://sigmausd.io/#/) the first UTxO-based stable coin - an instantiation of the [AgeUSD protocol](https://github.com/Emurgo/age-usd). The foundation on which a new era of digital finance will be built.
>
>Its economic model designed in partnership between IOHK, Ergo, and Emurgo maintains the conservative settings for collateral reserves and avoids the need for liquidations. Along with that, it supports a fully decentralised stablecoin emission setup. **Thus, SigmaUSD will offer the world a stable, simple, and decentralised stablecoin.**
{.is-success}

![sigmausd_overview.png](/sigmausd_overview.png)

**See these links for more information**
- [FAQ](/SigmaUSD/FAQ)
- [Detailed Overview](/SigmaUSD/Overview)
- [Noob tries to explain SigmaUSD/RSV (an attempt at an ELI5)](https://www.reddit.com/r/ergonauts/comments/nhjc1f/noob_tries_to_explain_sigmausdrsv_an_attempt_at/)
- [PSA: sigRSV is not a simple long position](https://www.reddit.com/r/ergonauts/comments/prxpag/psa_sigrsv_is_not_a_simple_long_position/)
- [ergo.watch](https://ergo.watch/sigmausd)


> Note  Transactions can fail when the oracle refreshes during (and the price changes). In this event the funds will be returned to your connected wallet.  Use this link for a refund anytime if your funds become 'stuck' in a proxy address:  `https://assm.sigmausd.io/return/your_address_set_in_ui/the_long_address_you_sent_to`
{.is-info}





# Use-cases
- Accepted in [Cryptocurrency Checkout](https://cryptocurrencycheckout.com/coin/sigmausd) 
- Mix SigUSD or SigRSV in [ErgoMixer](/ErgoMixer) the first non-custodial, non-interactive miner in the cryptocurrency space.
- Secure profits without interacting with exchanges.
- Short ERG
- Tips on Discord/Telegram/Reddit/etc
- SigUSD AuctionHouse


**Future**
- SigUSD on ErgoFund 
- SigUSD/USDx pairs on CEXs and DEXs


# Overview

> This is the simplest example possible to explain how the logic of the contract works (without fees) and not what happens in real world scenario. The value you can redeem for your SigRSV floats up and down based on transaction fees and profits/losses SigUSD holders take when withdrawing.
{.is-warning}

![sfpsbv4.png](/sfpsbv4.png)


## Advantages over MakerDAO
> **No liquidations!**
{.is-success}

Unlike Ethereum-based crypto-backed stablecoins, such as DAI, Emurgo introduces a Staticoin protocol-inspired design that does not rely on CDPs (Collateralized Debt Positions). The reason for this is the vulnerability of CDP-based protocols in terms of high volatility and blockchain congestion. As Emurgo states, "Black Thursday," when MakerDAO CDPs were triggered for liquidation due to volatility and then sold for $0 due to blockchain congestion that prevented others from bidding, demonstrated that a new design is needed. For SigmaUSD, this scenario is not possible.



# Resources
- [Erg/USD Explorer](https://explorer.ergoplatform.com/en/oracle-pool-state/ergusd) 


## Videos

- [Ergo Summit 2021 - The IOHK Perspective - Designing the AgeUSD StableCoin](https://youtu.be/zG-rxMCDIa0?t=9247)
- [Overview Video (with diagrams)](https://www.youtube.com/watch?v=O3hPEp3tzoU)
- [Youtube playlist](https://www.youtube.com/playlist?list=PL8-KVrs6vXLSu_rLQV5-Pu8389_PLd06q)


## Buying Guides

- https://youtu.be/FR1NCJbzn7w
- https://www.youtube.com/watch?v=cJuKRfRrTG4

## Calculators

- [sigusd.abchris.xyz](https://sigusd.abchris.xyz/)
- [Spreadhseet](https://docs.google.com/spreadsheets/d/1_lX0FrkIpNHmpMNKWrhhJpC93Wt5wco8oKlf-Wef9fw/edit?usp=sharing)

## Articles


- [Risk and reward mechanism](https://veriumfellow.medium.com/introduction-to-ergos-sigmausd-stablecoin-risk-and-reward-mechanism-18690b52d672)
- [AgeUSD Protocol: SigRSV and SigUSD](https://ergoplatform.org/en/blog/2021-07-30-ergos-ageusd-protocol-sigrsv-and-sigusd/)
- [Bearwhale Saga](https://ergoplatform.org/en/blog/2021-05-13-bearwhale-saga/)
- [SigmaUSD vs the competition.](https://curiaregiscrypto.medium.com/sigmausd-vs-the-competition-e70b23fe37a3)
- [SigmaUSD on Ergo - Privacy, Stability and Governance](https://curiaregiscrypto.medium.com/sigmausd-on-ergo-a36e0cdff743)
- [Building Ergo: How the AgeUSD stablecoin works](https://ergoplatform.org/en/blog/2021-02-05-building-ergo-how-the-ageusd-stablecoin-works/)



## Documentation

- The design was inspired by [StatiCoin](http://staticoin.com/whitepaper.pdf)
- [Documentation](https://github.com/Emurgo/age-usd)
- You can read the official [Emurgo announcement blog post here](https://ergoplatform.org/en/blog/2021_02_26-sigmausd-released/)


# SigmaUSD v1

This is v2, to read about v1 see these articles:

- [Finding The Right Balance](https://ergoplatform.org/en/blog/2021_03_04-finding-right-balance/)
- [Community Discussion on Reddit](https://www.reddit.com/r/ergonauts/comments/lx7an4/sigmausd_dao_bank_is_a_complex_beast_highlevel/gpr96fq/?context=3)
- [SigmaUSD (v1) Release](https://ergoplatform.org/en/blog/2021_02_26-sigmausd-released/)





# Infographics
## Reserve Ratio
![photo_2021-05-26_01.56.49.jpeg](/photo_2021-05-26_01.56.49.jpeg)

## Value
![](/photo_2021-05-19_10.01.10.jpeg =600x600)

## Technical

![screenshot_2021-02-25_at_19.14.01.png](/screenshot_2021-02-25_at_19.14.01.png)


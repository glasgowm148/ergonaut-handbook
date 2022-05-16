---
title: dApps/SigmaUSD
description: 
published: true
date: 2022-05-16T15:13:22.072Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:02:25.004Z
---

> Introducing [SigmaUSD.io](https://sigmausd.io/#/) the first UTxO-based stable coin - an instantiation of the [AgeUSD protocol](https://github.com/Emurgo/age-usd). The foundation on which a new era of digital finance will be built.
>
>Its economic model designed in partnership between IOHK, Ergo, and Emurgo maintains the conservative settings for collateral reserves and avoids the need for liquidations. Along with that, it supports a fully decentralised stablecoin emission setup. **Thus, SigmaUSD will offer the world a stable, simple, and decentralised stablecoin.**
{.is-success}

![sigmausd_overview.png](/sigmausd_overview.png)



# Overview


![sfpsbv4.png](/sfpsbv4.png)

# Resources

- [FAQ](/SigmaUSD/FAQ)
- [Detailed Overview](/SigmaUSD/Overview)
- [Erg/USD Explorer](https://explorer.ergoplatform.com/en/oracle-pool-state/ergusd) 
- [ergo.watch](https://ergo.watch/sigmausd)
- [Bank Wallet](https://explorer.ergoplatform.com/en/addresses)


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

- [AgeUSD Protocol: SigRSV and SigUSD](https://ergoplatform.org/en/blog/2021-07-30-ergos-ageusd-protocol-sigrsv-and-sigusd/)
- [Bearwhale Saga](https://ergoplatform.org/en/blog/2021-05-13-bearwhale-saga/)
- [SigmaUSD vs the competition.](https://curiaregiscrypto.medium.com/sigmausd-vs-the-competition-e70b23fe37a3)
- [SigmaUSD on Ergo - Privacy, Stability and Governance](https://curiaregiscrypto.medium.com/sigmausd-on-ergo-a36e0cdff743)
- [Building Ergo: How the AgeUSD stablecoin works](https://ergoplatform.org/en/blog/2021-02-05-building-ergo-how-the-ageusd-stablecoin-works/)
- [Risk and reward mechanism](https://veriumfellow.medium.com/introduction-to-ergos-sigmausd-stablecoin-risk-and-reward-mechanism-18690b52d672)

**Threads**

- [Noob tries to explain SigmaUSD/RSV (an attempt at an ELI5)](https://www.reddit.com/r/ergonauts/comments/nhjc1f/noob_tries_to_explain_sigmausdrsv_an_attempt_at/)
- [PSA: sigRSV is not a simple long position](https://www.reddit.com/r/ergonauts/comments/prxpag/psa_sigrsv_is_not_a_simple_long_position/)


## Documentation

- The design was inspired by [StatiCoin](http://staticoin.com/whitepaper.pdf)
- [Documentation](https://github.com/Emurgo/age-usd)
- You can read the official [Emurgo announcement blog post here](https://ergoplatform.org/en/blog/2021_02_26-sigmausd-released/)

## Troubleshooting

## My funds are stuck

Use this link for a refund anytime if your funds are stuck in a proxy address: 
```
https://assm.sigmausd.io/return/your_address_set_in_ui/the_long_address_you_sent_to
````


## Other Stablecoins

- [SigmaUSD vs the competition](https://curiaregiscrypto.medium.com/sigmausd-vs-the-competition-e70b23fe37a3
)

**Use-cases**
- Accepted in [Cryptocurrency Checkout](https://cryptocurrencycheckout.com/coin/sigmausd) 
- Mix SigUSD or SigRSV in [ErgoMixer](/ErgoMixer) the first non-custodial, non-interactive miner in the cryptocurrency space.
- Secure profits without interacting with exchanges.
- Short ERG
- Tips on Discord/Telegram/Reddit/etc
- SigUSD AuctionHouse
- Deposit liquidity in ErgoMixer and redeem a percentage of the trading fees. 


**Future**
- SigUSD on ErgoFund 
- SigUSD/USDx pairs on CEXs and DEXs


## Advantages over MakerDAO
> **No liquidations!**
{.is-success}

Unlike Ethereum-based crypto-backed stablecoins, such as DAI, Emurgo introduces a Staticoin protocol-inspired design that does not rely on CDPs (Collateralized Debt Positions). The reason for this is the vulnerability of CDP-based protocols in terms of high volatility and blockchain congestion. As Emurgo states, "Black Thursday," when MakerDAO CDPs were triggered for liquidation due to volatility and then sold for $0 due to blockchain congestion that prevented others from bidding, demonstrated that a new design is needed. For SigmaUSD, this scenario is not possible.

## Advantages over UST

SigUSD is over-collateralised, every sigusd is backed by 3$ currently. Everyone can see that there is money in the bank. This stops a bank run at its inception. The breaking point of the peg is explicit and open for anyone to see. With UST, you have no idea, which gives you an incentive to get out first.


- Luna supply depends on terra usage, Ergo does not. Burning luna when trend is up, pumps its price. However, when trend is down, luna price will dump harder, because more luna is printed. 

- collateral ratio for sigusd is higher. This means that the capital efficiency (less collateral tied for each stablecoin) is better for terra. That is why luna/terra can offer better yield. 

However, this means that luna/terra needs an additional mechanism to ensure stability. When collateral (luna) value drops, someone needs to step in to stabilize it. Those people are incentivized with promises of larger profits in the future. This assumes that there will always be people who believe that the protocol survives the crash. No one knows at which price point of luna the trust disappears. This creates a seed for a bank run. Everyone wants to take their  stablecoin out faster than others, if there is any doubt.

In contrast, sigusd shows explicitly, when the peg is going to be lost. No one needs to guess how long the protocol can last.

credit to `ile` on Telegram who's been warning of this bank-run since Lunar's inception.



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


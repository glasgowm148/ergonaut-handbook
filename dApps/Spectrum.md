---
title: Spectrum (ex-ErgoDEX)
description: Spectrum is a native cross-chain DeFi ecosystem
published: false
date: 2022-09-06T17:51:38.805Z
tags: 
editor: markdown
dateCreated: 2022-09-06T17:51:38.805Z
---

## SpectrumLabs
### Introduction
#### **What is Spectrum.DEX?​**

Spectrum.DEX is a non-custodial decentralized exchange that allows a quick, effortless, and secure transfer of liquidity inside and between the **Ergo** and **Cardano** networks. The eUTXO model gives the unique possibility to have shared liquidity among different networks. **Spectrum.DEX will eventually feature a full AMM, Order Book and more.**

Spectrum.DEX is an open-source DeFi product which take a part in both Ergo and Cardano platforms and as a consequence exists for purposes of both communities. You can imagine Spectrum.DEX infrastructure like the following:

- **Spectrum Labs**: the team of developers who are developing and maintaining Spectrum.DEX protocol, user interface and other products;
- **The Spectrum.DEX Protocol**: a set of smart contracts that create an automated market maker and order book;
- **Spectrum.DEX User Interface (UI)**: a web (or mobile) interface which provides access in conjunction with the protocol;
- **Spectrum.DEX Execution Bots**xxxxxxx: off-chain software whose function is to execute DEX orders and works in a completely decentralized manner.
_______
**ErgoDex has rebranded to [Spectrum Labs!](https://ergonaut.space/en/dApps/ergodex)**



- [Medium article](https://spectrumlabs.medium.com/now-we-are-spectrum-eaf17a2b65e) | reasons for Ergodex-->Spectrum Labs rebrand  
- [r/SpectrumLabs](https://www.reddit.com/r/SpectrumLabs/) | new subreddit
- [spectrum.fi](https://spectrum.fi/)  | new landing-page URL for project/ DEX
- [SpectrumDocs](https://docs.spectrum.fi/) | detailed overview and usage guides

> "Over time we realized that the ambitions of our team went beyond just a DEX, so we decided to transform our project into something more. We called it Spectrum." ![spectrumecosystem-from-medium-article.jpeg](/spectrumecosystem-from-medium-article.jpeg)
{.is-info}



> ErgoDex is now [Spectrum](https://spectrum.fi/)!
All the info below was written **prior** to the Spectrum rebrand. Complete SpectrumLabs page coming *soon*...
{.is-success}


_____________
## ErgoDex 
![timeline_project_1920x1080_logo_update_06_28_21.png](/timeline_project_1920x1080_logo_update_06_28_21.png)

> [EIP-0014: Decentalized Exchange Contracts](https://github.com/ergoplatform/eips/pull/27)
{.is-info}

[See the slide deck](https://ergonaut.space/ergodex.pdf)

Ergo has built-in atomic exchange for its custom, first-class citizen tokens built into its core. ErgoDex is a *Uniswap-like* AMM-based Decentralised Exchange (DEX) which allows for direct peer-to-peer cryptocurrency transactions, reducing the need for centralised exchanges.

In ErgoSwap anyone can discover the match for orders and then submit the swap transaction, while getting incentives (including offchain services). Demonstrating concepts of earning without mining rig with Ergo dApps while supporting decentralization and privacy.

# EIP0014

Exchanging without trusted parties is a one of the most basic primitive for decentralized finance. As such, basic single-chain swap contracts were introduced early in the ErgoScript whitepaper. Then a lot of other order contracts appeared: with partial filling, buyback guarantee and so forth. Such contracts are usually composable,

While swap order contracts allows for orderbook-based decentralized exchanges (DEXes), now popular AMM-based DEXes (Automated Market Maker) are also possible on Ergo.

Interestingly, unlike other known blockchains, thanks to the extended UTXO model, liquidity pool contracts for AMM-based DEXes can be combined with order contracts (for orderbook-based DEXes). This gives unique possibility to have shared liquidity among different types of exchanges on top of the Ergo blockchain.

This PR provides known DEX contracts for both orderbook-based and AMM-based DEXes, and also provides info on their composability.

![screenshot_2021-02-24_at_09.55.05.png](/screenshot_2021-02-24_at_09.55.05.png)



---
title: ErgoDEX
description: 
published: true
date: 2021-05-07T16:13:28.983Z
tags: 
editor: markdown
dateCreated: 2021-04-24T11:14:01.510Z
---

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

# Gravity

Above the standard and private swaps, Gravity will be implemented - making ERC20 tokens possible. 

1. Core in Q1
1. Swaps & Gateways in Q2
1. Full-fledged DEX ~2022


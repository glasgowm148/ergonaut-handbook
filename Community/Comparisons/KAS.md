---
title: Ergo vs KAS
description: 
published: true
date: 2023-08-07T09:26:42.966Z
tags: 
editor: markdown
dateCreated: 2023-08-07T09:26:17.272Z
---

# Ergo vs Kaspa


| Feature | Ergo (ERG) | Kaspa (KSP) |
|---------|------------|-------------|
| **Consensus Mechanism** | Autolykos (Proof-of-Work) | ghostDAG protocol |
| **Smart Contracts** | Yes, with ErgoScript | No |
| **Privacy Features** | Yes, includes ring signatures and zero-knowledge proofs | No |
| **Scalability** | Aims to solve scalability with NiPoPoWs, eUTXO model | Aims to solve scalability issues with ghostDAG protocol |
| **Use Cases** | Financial contracts | Fast transactions  |
| **ASIC-Resistant** | Yes | No, ASICs are on the network |


> kushti khushi, [7 Aug 2023](https://t.me/ergoplatform/419156):
>
> Checked yesterday Kaspa core code a bit, I doubt introduction of smart contracts will be simple, on top of input signing with different sighash option taken from bitcoin they have
> 
> Also, have some doubts about muhash they are using for state authentication, and not clear why incremental hash was used instead of authenticated dictionary
>
> And verification dilemma in the presence of dag could hit hard, have to check how it was accounted in ghostdag paper and its continuations, probably just skipped
>
> Yonatan has an idea back in 2017 to have client side validation, so miners in this case can include double spends and other invalid but well formed transactions

> Which is solving verification dilemma for miners at least but a very different beast from blockchains we know

> But Kaspa is so extreme from initial investigation
---
title: UTXO
description: A description of the UTXO model
published: true
date: 2022-09-20T15:00:01.725Z
tags: 
editor: markdown
dateCreated: 2021-12-31T22:42:53.074Z
---

> Ergo uses the extended-UTXO or [eUTXO](https://ergonaut.space/en/Glossary/eUTXO) model, enabling powerful turing-complete smart contracts to be implemented securely and efficiently,  on-top of Bitcoin's original UTXO model.
{.is-success}
# UTXO

- An *Unspent Transaction Output*, or UTXO, is the result of a transaction that a user receives and is able to spend in the future. This is true because, as the name suggests, it is the unspent output of a transaction. Note that every UTXO can only be spent once. At that point, the UTXO is no longer unspent, meaning that it cannot be used again in the future.

- Accordingly, the UTXO *Model* is a way of organizing a blockchain's ledger such that no funds are spent twice, avoiding the double spending problem. Once a UTXO is spent, one (or more) new UTXO are created as a result of that transaction. The new UTXO are created and sent to the appropriate wallet(s).

- Broadly speaking, the UTXO model is one variety of blockchain protocol. While there's no mention of UTXO in the Bitcoin white paper, the UTXO model was first developed by Satoshi Nakamoto when the Bitcoin blockchain was first published. The original Bitcoin script relies heavily on UTXO to check whether or not a particular wallet has sufficient funds to execute a requested transaction.

**SOURCE: Our friend and fellow member of the UTXO Alliance, Komodo Platform's [What's a UTXO?](https://komodoplatform.com/en/academy/whats-utxo/) page.**



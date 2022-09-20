---
title: Turing-complete
description: definition and examples
published: true
date: 2022-09-20T16:41:40.487Z
tags: 
editor: markdown
dateCreated: 2022-09-20T15:14:55.658Z
---

# Turing-complete
## Description

From [Wikipedia](https://en.wikipedia.org/wiki/Turing_completeness#):

- In colloquial usage, the terms "Turing-complete" and "Turing-equivalent" are used to mean that any real-world general-purpose computer or computer language can approximately simulate the computational aspects of any other real-world general-purpose computer or computer language.

- The Church–Turing thesis states that this is a law of mathematics – that a universal Turing machine can, *in principle*, perform any calculation that any other programmable computer can. This says nothing about the effort needed to write the program, or the time it may take for the machine to perform the calculation, or any abilities the machine may possess that have nothing to do with computation.
____
## Turing-complete Smart Contracts

- Ethereum is an exceptional platform, but there are things it does not do well. Its Turing-complete smart contracts are powerful but dangerous – as incidents from The DAO to the Parity wallet exploits have proven, with tens of millions of dollars in collateral damage. With complexity comes uncertainty and potentially catastrophic vulnerabilities. Contracts can be expensive to run, and depending on network conditions, may execute unpredictably – or not.
- Ergo on the flip side, [extends UTXO](https://ergonaut.space/en/Glossary/eUTXO) to enable Turing-completeness (by iterating processes across multiple blocks) while limiting the complexity of the [ErgoScript](https://ergonaut.space/en/Glossary/ErgoScript) language itself. **The same expressive power is achieved in a different and more semantically sound way.** That means Ergo can support versatile [dApps](/en/dApps/dApps-Index) that run predictably, with known costs, and don't have any of the dangers of unrestricted functionality.
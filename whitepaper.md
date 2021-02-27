---
title: Whitepaper
description: 
published: true
date: 2021-02-24T19:50:20.214Z
tags: 
editor: undefined
dateCreated: 2021-02-24T08:09:20.563Z
---

# Whitepaper
>  Ergo is following the fundamental approach and use stable well-tested solutions, even if that leads to slower short-term innovations. Most of Ergo solutions are formalized in papers presented at peer-reviewed conferences and have been widely discussed in the community.
{.is-info}

Visit [ergoplatform.org](https://ergoplatform.org/en/documents/) for a full list of publications


## Whitepaper - Bitesize Edition 🍔
Blockchain technology has so far proved to be a secure way of maintaining a public transaction ledger. But this resilience comes at a cost and has not yet been proven for existing systems in the long-run at economy-wide scale.

To use a blockchain without any trust, its participants should check each other by downloading and processing all the transactions in the network, utilizing network resources.

Ergo is based on the UTXO model and provides a convenient way to implement financial applications covering an overwhelming majority of public blockchain use-cases. It aims to provide a way for further improvements without any breaking changes.
and this is exactly what Ergo seeks to accomplish.

### 🚀 **Ergo Vision**

**It is suitable for several applications but its main focus is to provide an efficient, secure and easy way to implement financial contracts.**

In case of intentional violation of any of these principles, the resulting protocol should not be called Ergo. Ergo is the base layer to applications that will be built on top of it.

The Ergo protocol is very flexible and may be changed in the future by the community.

### 🔐 **Ergo State**

Ergo follows Bitcoin's UTXO design and represents the snapshots using onetime coins. In addition to monetary value and protecting script, an Ergo one-time coin, called a box, also contains userdefined data. An Ergo block also stores an authenticating digest, called the stateRoot, of the global state after applying the block.

Ergo miners are required to generate proofs of block modifications and a hash of this proof is included into the block header along with the digest of the resulting state.
For instance, Patricia trie used in Ethereum for the same purpose
> **Thus, Ergo state provides an efficient and secure way to prove the existence or non-existence of certain elements in the tree, as well as proofs of tree modifications.**
{.is-success}

### 🧱 **Resiliency and Survivability**

Ergo is a platform for contractual money. It should also support long-term contracts for a period of at least an average person's lifetime. Even young existing smart contract platforms are experiencing issues with performance degradation and adaptability to external conditions.

This leads to a situation where the cryptocurrency depends on a small group of developers to provide a fixing hard-fork, or the cryptocurrency won't survive. Ergo's approach here is to use stable well-tested solutions, even if they lead to slower short-term innovations.

### 💰 Contractual Money

In our opinion, the overwhelming majority of use-cases for public blockchains are for financial applications, which do not require Turing-completeness. Ergo applications are defined in terms of protecting scripts built into boxes, which may also contain data involved in the execution. We use the term contractual money to define Ergs (and secondary tokens) whose usage is bounded by a contract.

Most of the solutions used in Ergo are formalized in papers presented at peer-reviewed conferences

Ergo uses an authenticated state 4 and for transactions included in a block, a client may download a proof of their correctness.
This header alone allows for validation of the work done on it and a headers-chain is enough for best chain selection and synchronization with the network.

A large state size leads to serious security issues because when the state does not fit in random-access memory, an adversary can generate transactions whose validation become very slow due to required random access to the miner's storage.


### Autolykos Consensus Protocol
The original PoW protocol with the longest chain rule is still in demand due to its simplicity, high-security guarantees, and friendliness to light clients.

A decade of extensive testing has revealed several problems with the original one-CPU-one-vote idea.

The first known problem of a PoW system is the development of specialized hardware, which allows a small group of ASIC-equipped miners to solve PoW puzzles orders of magnitude faster than everyone else.




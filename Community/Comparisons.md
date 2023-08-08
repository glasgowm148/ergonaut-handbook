---
title: Comparisons
description: 
published: true
date: 2023-08-08T13:04:29.261Z
tags: 
editor: markdown
dateCreated: 2023-03-15T12:29:22.180Z
---

# Smart Contract Platform Comparison Guide

These comparisons aim to be neutral, but may contain misunderstandings; if you're landing on this page from one of the communities listed - feel free to sign up to this site and make clarifying edits!

See also the [Crypto Comparison Table](https://docs.google.com/spreadsheets/d/1SBCylFAuJRcvZ47obGXfQz19bHDYdaJznnzemcaBgWk/edit?usp=sharing) sheet where various projects are categorised and ranked. 

# extended UTXO

Below are some of our closest competitors on the technical front. Detailed comparison pages are linked where available, please add to this resource!


| Cryptocurrency   | Ticker | Consensus  | Contracts |  Features  |  Model | 
|------------------|--------|------------|-----------|------------|--------|
| Ergo             | ERG    | Proof of Work       | Box Model  | Sigma protocols, eUTXO model, and focus on financial contracts | eUTXO         |               
| [Nervos CKB](https://ergonaut.space/en/Community/Comparisons/CKB)| CKB    | Proof of Work       |  CKB-VM | Common Knowledge Base, layered architecture, and focus on scalability and security | UTXO |
| [Alephium](https://ergonaut.space/en/Community/Comparisons/ALPH)             | ALPH    | Proof of Less Work |Alphred VM| Fast-PoW | stateful-UTXO |
| [Verge](https://ergonaut.space/en/Community/Comparisons/XVG)            | XVG    | Proof of Work       |*(Planned)* [MiniScript](https://vergecurrency.com/key-tech/)      | Focus on privacy, multi-algorithm mining, and fast transactions | UTXO |

# Virtual Machine

Below are some of our closest competitors on the technical front. Detailed comparison pages are linked where available, please add to this resource!


| Cryptocurrency   | Ticker | Consensus  | Contracts |  Features  |  Model | 
|------------------|--------|------------|-----------|------------|--------|
| [Nervos CKB](https://ergonaut.space/en/Community/Comparisons/CKB)| CKB    | Proof of Work       |  CKB-VM | Common Knowledge Base, layered architecture, and focus on scalability and security | UTXO |
| [Alephium](https://ergonaut.space/en/Community/Comparisons/ALPH)             | ALPH    | Proof of Less Work |Alphred VM| Fast-PoW | stateful-UTXO |


# Assets-based 

DigiByte, Ravencoin, and Flux, like Ergo, do not rely on a traditional virtual machine (VM) for their primary functionalities. Instead, they have implemented specialized systems or protocols tailored to their specific use cases.

| Aspect/Feature |  Ergo |[Digibyte](https://ergonaut.space/en/Community/Comparisons/DGB) | [RavenCoin](https://ergonaut.space/en/Community/Comparisons/RVN) | [Flux](https://ergonaut.space/en/Community/Comparisons/FLUX) |
|----------------|----------|-----------|------|------|
| **Primary Focus** | Financial contracts and decentralized applications | DigiAssets for asset issuance and more | Asset issuance and transfer | Decentralized computational infrastructure | 
| **Execution Environment** | eUTXO model with ErgoScript | Native DigiByte blockchain | Native Ravencoin protocol | Native Flux blockchain |
| **Smart Contracts** | ErgoScript with multi-stage protocol for Turing completeness | Limited programmable conditions | Primarily asset-focused, not versatile smart contracts | Not the primary focus | 
| **Asset System** | eUTXO model allows for token issuance and more |DigiAssets | Asset Layer | Flux Assets | 



# Exotic Consensus'

While all these models use PoW, the way they achieve consensus and handle transactions varies, leading to different trade-offs in terms of security, speed, and decentralization. Here's a comparison table of the consensus mechanisms compared to Ergo's eUTXO model:

| Feature/Model | Ergo | [Conflux](https://ergonaut.space/en/Community/Comparisons/CFX) | [Syscoin](https://ergonaut.space/en/Community/Comparisons/SYS) | [Kaspa](https://ergonaut.space/en/Community/Comparisons/KAS) |
|---------------|--------------|-------------------|--------------------|----------------------|
| **Consensus** | eUTXO | Tree-Graph (TG) | Z-DAG | GHOSTDAG |
| **Contracts** | Box Model | VM | NEVM | *Planned* |
| **Security** | Battle-tested with known security assumptions. | Newer mechanism; long-term security implications not as well-understood. | Still a topic of research under different network conditions. | Different security model from traditional blockchains; requires more research. |
| **Decentralization** | Ensures power isn't concentrated; anyone can participate. | Aims for high throughput without sacrificing decentralization. | Not inherently tied to decentralization. | Can handle concurrent blocks, but decentralization varies by implementation. |
| **Finality** | Probabilistic finality; becomes more secure with more confirmations. | Achieves consensus faster than traditional blockchains. | Fast transactions, but finality varies by implementation. | Provides a partial order of blocks for faster consensus. |
| **Efficiency** | Optimized for smart contracts and complex financial transactions. | Optimized for high throughput. | Designed for fast microtransactions. | Aims for faster consensus than traditional blockchains. |
| **Drawbacks** | Energy-intensive due to PoW, but offers robust security. | Long-term security implications are still being studied. | Security under adversarial scenarios is still being researched. | Security model is different from traditional blockchains. |






# PoW > Smart Contracts > Account Model


| Cryptocurrency   | Ticker | Consensus  | Contracts | Fork of                  | Features                                  |  Model | 
|------------------|--------|---------------------|-----------------|------------------------|---------------------------------------------------|------------------|
| [Ethereum Classic](https://ergonaut.space/en/Community/Comparisons/ETC) | ETC    | Proof of Work       | Yes             | Ethereum               | Ethereum's original chain, focus on immutability and decentralization | Account-based |
| [Kadena](https://ergonaut.space/en/Community/Comparisons/KDA) | KDA    | Proof of Work       | Yes             |                |  | Account-based 
| [Ubiq](https://ergonaut.space/en/Community/Comparisons/UBQ)              | UBQ    | Proof of Work       | Yes             | Ethereum               | Ethereum fork with modified parameters, focus on stability and enterprise use | Account-based |
| [Expanse](https://ergonaut.space/en/Community/Comparisons/EXP)           | EXP    | Proof of Work       | Yes             | Ethereum               | Ethereum fork, focus on decentralized applications and governance | Account-based |
| [Rootstock](https://ergonaut.space/en/Community/Comparisons/RSK)   | RSK   | Merge-mined with Bitcoin | Yes      | Bitcoin                | Smart contracts on Bitcoin, secured by Bitcoin's mining power | Account-based |

# Comparison: VM Approach vs. Ergo's Approach

| Aspect/Feature | Virtual Machine (e.g., Ethereum's EVM) | Ergo (eUTXO + ErgoScript) |
|----------------|----------------------------------------|---------------------------|
| **Execution Environment** | Simulates a computer system. | Processes transactions directly on the blockchain. |
| **Turing Completeness** | Yes, VMs like EVM are Turing complete. | ErgoScript is non-Turing complete, but  multi-stage protocols enable Turing completeness. |
| **Resource Management** | Uses a "gas" mechanism to prevent excessive computation. | Predictable execution cost due to non-Turing complete nature of ErgoScript. |
| **State Management** | Maintains a global state that's updated after every transaction. | Uses the eUTXO model which is inherently stateless. Each transaction refers to previous UTXOs and produces new ones. |
| **Complexity & Versatility** | Can run complex and versatile smart contracts. | ErgoScript ensures predictability, but the multi-stage protocol allows for complex operations. |
| **Data Model** | Account-based model. | Extended UTXO model where UTXOs can carry additional data. |

This table provides a side-by-side comparison of the key features and differences between a traditional virtual machine approach and Ergo's approach. Both methods have their strengths and trade-offs, and the choice between them would depend on specific use cases and requirements.



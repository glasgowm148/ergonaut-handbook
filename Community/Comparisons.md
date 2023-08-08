---
title: Comparisons
description: 
published: true
date: 2023-08-08T09:13:53.473Z
tags: 
editor: markdown
dateCreated: 2023-03-15T12:29:22.180Z
---

# Smart Contract Platform Comparison Guide

These comparisons aim to be neutral, but may contain misunderstandings; if you're landing on this page from one of the communities listed - feel free to sign up to this site and make clarifying edits!

# PoW > Smart Contracts > UTXO

Below are some of our closest competitors on the technical front. Detailed comparison pages are linked where available, please add to this resource!


| Cryptocurrency   | Ticker | Consensus  | Contracts |  Features  |  Model | 
|------------------|--------|------------|-----------|------------|--------|
| Ergo             | ERG    | Proof of Work       | Assets+SC  | Sigma protocols, eUTXO model, and focus on financial contracts | eUTXO         |               
| [Nervos CKB](https://ergonaut.space/en/Community/Comparisons/CKB)| CKB    | Proof of Work       |  CKB-VM | Common Knowledge Base, layered architecture, and focus on scalability and security | sUTXO |
| [Verge](https://ergonaut.space/en/Community/Comparisons/XVG)            | XVG    | Proof of Work       |Planned     | Focus on privacy, multi-algorithm mining, and fast transactions | UTXO |
| [Digibyte](https://ergonaut.space/en/Community/Comparisons/DGB)         | DGB    | Proof of Work       | DigiAssets | Multi-algorithm mining, focus on security and decentralization | UTXO |
| [RavenCoin](https://ergonaut.space/en/Community/Comparisons/RVN)        | RVN    | Proof of Work       |Assets  | P2P Assets | UTXO |
| [Flux](https://ergonaut.space/en/Community/Comparisons/FLUX)             | FLUX   | Proof of Work       | Cloud Infrastructure | Scalable infrastructure, parallel assets, and node incentivization | UTXO |

# PoW > Smart Contracts > Other

Here's a comparison table of the consensus mechanisms compared to Ergo's eUTXO model:


| Feature/Model | eUTXO (Ergo) | T-GRAPH (Conflux) | DAG (Syscoin) | GhostDAG (Kaspa) |
|---------------|--------------|-------------------|--------------------|----------------------|
| **Security** | Battle-tested with known security assumptions. | Newer mechanism; long-term security implications not as well-understood. | Still a topic of research under different network conditions. | Different security model from traditional blockchains; requires more research. |
| **Decentralization** | Ensures power isn't concentrated; anyone can participate. | Aims for high throughput without sacrificing decentralization. | Not inherently tied to decentralization. | Can handle concurrent blocks, but decentralization varies by implementation. |
| **Finality** | Probabilistic finality; becomes more secure with more confirmations. | Achieves consensus faster than traditional blockchains. | Fast transactions, but finality varies by implementation. | Provides a partial order of blocks for faster consensus. |
| **Efficiency** | Optimized for smart contracts and complex financial transactions. | Optimized for high throughput. | Designed for fast microtransactions. | Aims for faster consensus than traditional blockchains. |
| **Drawbacks** | Energy-intensive due to PoW, but offers robust security. | Long-term security implications are still being studied. | Security under adversarial scenarios is still being researched. | Security model is different from traditional blockchains. |

While all these models use PoW, the way they achieve consensus and handle transactions varies, leading to different trade-offs in terms of security, speed, and decentralization.


| Cryptocurrency   | Ticker | Consensus  | Contracts |  Features  |  Model | 
|------------------|--------|------------|-----------|------------|--------|
| [Kaspa](https://ergonaut.space/en/Community/Comparisons/KAS)| KAS| Proof of Work|Planned| high throughput, and fast confirmation times | GHOSTDAG| 
| [Syscoin](https://ergonaut.space/en/Community/Comparisons/SYS)          | SYS    | Proof of Work       | NEVM | Asset/token creation, decentralized marketplace | Z-DAG |  
| [Conflux](https://ergonaut.space/en/Community/Comparisons/CFX)             | CFX    | Proof of Work |VM| Fast-PoW | Tree-Graph (TG) |

# PoW > Smart Contracts > Account Model


| Cryptocurrency   | Ticker | Consensus  | Contracts | Fork of                  | Features                                  |  Model | 
|------------------|--------|---------------------|-----------------|------------------------|---------------------------------------------------|------------------|
| [Ethereum Classic](https://ergonaut.space/en/Community/Comparisons/ETC) | ETC    | Proof of Work       | Yes             | Ethereum               | Ethereum's original chain, focus on immutability and decentralization | Account-based |
| [Kadena](https://ergonaut.space/en/Community/Comparisons/KDA) | KDA    | Proof of Work       | Yes             |                |  | Account-based 
| [Ubiq](https://ergonaut.space/en/Community/Comparisons/UBQ)              | UBQ    | Proof of Work       | Yes             | Ethereum               | Ethereum fork with modified parameters, focus on stability and enterprise use | Account-based |
| [Expanse](https://ergonaut.space/en/Community/Comparisons/EXP)           | EXP    | Proof of Work       | Yes             | Ethereum               | Ethereum fork, focus on decentralized applications and governance | Account-based |
| [Rootstock](https://ergonaut.space/en/Community/Comparisons/RSK)   | RSK   | Merge-mined with Bitcoin | Yes      | Bitcoin                | Smart contracts on Bitcoin, secured by Bitcoin's mining power | Account-based |



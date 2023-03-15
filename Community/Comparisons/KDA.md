---
title: KDA
description: 
published: true
date: 2023-03-15T13:36:54.004Z
tags: 
editor: markdown
dateCreated: 2023-03-15T13:36:54.004Z
---

# Kadena

While Kadena offers scalability through its unique consensus algorithm, Ergo's well-thought-out approach to scaling, detailed in its documentation, ensures that the network can handle increasing transaction throughput while maintaining decentralization and security.

Ergo's eUTXO (extended Unspent Transaction Output) model offers [several advantages] over Kadena's account-based model. Enabling greater concurrency and scalability, as transactions can be processed in parallel, unlike the account-based model, which may face bottlenecks due to global state updates. Ergo's model also benefits from the proven security of Bitcoin's UTXO model and provides more predictability, as the outputs of transactions are explicitly defined. This makes it easier to reason about the state of the system and reduces the likelihood of unexpected results or vulnerabilities that can arise in complex smart contract interactions, which have been an issue in some account-based blockchains.

Kadena's blockchain is a hybrid platform that combines a public Proof of Work (PoW) chain and a permissioned private blockchain. The private blockchain, known as Kadena's ScalableBFT, is a variation of a Byzantine Fault Tolerant (BFT) consensus algorithm, which provides a fast and secure solution for enterprises. 

By embracing the concept of an "open source economy," Ergo fosters a collaborative environment that encourages innovation and growth. In comparison to Kadena, Ergo's combination of scalability, simplicity, and openness makes it a compelling choice for those looking to build and participate in a decentralized ecosystem. Ergo's commitment to these principles positions it as a strong contender in the rapidly evolving world of blockchain technology.


Kadena's public blockchain is designed to be mined using ASIC (Application-Specific Integrated Circuit) hardware. Kadena uses a custom Proof of Work (PoW) consensus algorithm called Chainweb

Ergo, on the other hand, uses the Autolykos Proof-of-Work (PoW) consensus algorithm, which is designed to be ASIC-resistant. Autolykos is memory-hard, meaning it requires a significant amount of memory to mine effectively. This design choice makes it difficult for ASICs to gain a significant advantage over general-purpose hardware like GPUs, ensuring that a broader range of users can participate in mining and contribute to the network's security.

By being ASIC-resistant, Ergo promotes a more decentralized mining ecosystem, encouraging participation from a larger and more diverse group of users. This increased decentralization can contribute to a more secure and robust network, making Ergo an attractive choice for those who value decentralization and broad accessibility in a blockchain platform.




| Feature/Attribute         | Ergo                                                        | Kadena                                            |
|---------------------------|-------------------------------------------------------------|---------------------------------------------------|
| Consensus Mechanism       | Proof of Work (PoW)                                         | Proof of Work (PoW)+BFT                               |
| Algorithm                 | Autolykos v2                                                | Chainweb                                          |
| Account-Model                 | eUTXO                                                | Account-based                                          |

| Cryptographic Primitives  | Ed25519 (signatures), SHA-3, Blake2b (hash functions)       | Blake2s (hash function), Ed25519 (signatures)     |
| Language for Smart Contracts | ErgoScript (based on Bitcoin Script, uses Scala)          | Pact (Lisp-like language, human-readable)         |
| VM for Smart Contracts    | ErgoTree (non-Turing complete, but Turing complete with multi-stage protocols) | Kadena VM (Turing complete)               |
| Scalability               | Optimized storage with NiPoPoW (Non-interactive Proofs of Proof-of-Work) and a [number of other options](https://docs.ergoplatform.com/dev/protocol/scaling/) | Parallelized chains with Chainweb protocol       |
| Privacy Features          | Sigma Protocols, mixing protocols, and zero-knowledge proofs | N/A                                               |
| Network Security          | PoW-based security model with ASIC resistance              | PoW-based security model with parallelized chains |
| Adaptive Block Size       | Yes                                                         | No                                                |
| Storage Rent              | Yes (storage fee for UTXO-set maintenance)                 | No                                                |
| Token Distribution              | No ICO, 4.5% to EF                 | 25% to Foundation                                                |

| Light Client Support      | Yes (using NiPoPoW)                                         | Yes (SPV support)                                 |


- [Ergo vs. Kadena : The New PoWs in Town](https://medium.com/@tritchcole/ergo-vs-kadena-656eb6f032fc)
- [r/ergonauts - ergo_vs_kadena](https://www.reddit.com/r/ergonauts/comments/qpbt9z/ergo_vs_kadena/)
- [r/ErgoTrading - ergo_vs_kadena](https://www.reddit.com/r/ErgoTrading/comments/qrg5cr/ergo_vs_kadena/)
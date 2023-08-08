---
title: Nervos CKB
description: 
published: true
date: 2023-08-08T13:11:23.602Z
tags: 
editor: markdown
dateCreated: 2023-08-08T09:16:19.415Z
---

# Nervos CKB


| Feature | Ergo (ERG) | Nervos CKB |
|---------|------------|------------|
| **Consensus Mechanism** | Autolykos (Proof-of-Work) | Eaglesong (Proof-of-Work) |
| **Smart Contracts** | Yes, with [ErgoScript](https://docs.ergoplatform.com/dev/scs/ergoscript/) | Yes, with CKB-VM (RISC-V based) |
| **Privacy Features** | Yes, includes ring signatures and zero-knowledge proofs | No |
| **Scalability** | Aims to solve [scalability with the power of eUTXO, NiPoPoWs and other novel features](https://docs.ergoplatform.com/dev/protocol/scaling/) | Layer 1 scalability with the "Common Knowledge Base" model |
| **Use Cases** | Financial contracts | Multi-asset store of value, smart contracts |
| **ASIC-Resistant** | Yes | No (Eaglesong ASIC mining) |
| **Language-base** | JVM | C, Rust |
| **Public Distribution** | ~95% | TBC |

## Cell Model vs Box Model

The concepts of Nervos CKB's "Cell" model and Ergo's "Box" model are similar in many ways, both being evolutions of the UTXO model. However, there are differences in their implementations and the ecosystems in which they operate. Let's break down the similarities and differences:

### Nervos CKB's Cell Model:

1. **Cell**: In Nervos, the fundamental unit is a "Cell," which can contain data, including tokens, smart contract code, or other arbitrary data.
2. **State Storage**: The state in Nervos is stored in these cells. When a transaction occurs, it consumes input cells and produces new output cells.
3. **CKB-VM**: The CKB-VM is the virtual machine in Nervos that ensures the rules (or scripts) associated with cells are correctly followed. It verifies that transactions are valid by executing these rules.

### Ergo's Box Model:

1. **Box**: In Ergo, the fundamental unit is a "Box." Like Nervos' cells, boxes can contain tokens and arbitrary data. They also contain "ErgoScript" code, which defines the conditions under which the box can be spent.
2. **State Storage**: The state in Ergo is represented by the UTXO set, where each UTXO is a box. Transactions consume boxes as inputs and produce new boxes as outputs.
3. **No Traditional VM**: Ergo doesn't have a traditional VM like Ethereum's EVM or Nervos' CKB-VM. Instead, it uses ErgoScript, a non-Turing complete language, to define the spending conditions of boxes. ErgoScript is executed directly on the blockchain.

### Comparison:

- **Similarities**: Both models are evolutions of the UTXO model, where the fundamental units (cells or boxes) can contain tokens and arbitrary data. Both models are stateless, meaning transactions refer to previous units (cells or boxes) and produce new ones.
  
- **Differences**: The primary difference lies in how smart contract logic is executed. Nervos has the CKB-VM, a virtual machine that operates on cells and ensures their associated rules are followed. Ergo, on the other hand, doesn't have a traditional VM. Instead, it uses ErgoScript to define the conditions under which boxes can be spent, and this script is executed directly on the blockchain.

### Is Ergo's Box Model a VM?

In a traditional sense, no. A virtual machine typically simulates a computer system, allowing for the execution of code in a controlled environment. Ergo's approach is different. While ErgoScript does execute logic, it does so directly on the blockchain without the intermediary of a traditional VM. ErgoScript defines the conditions for box spending, and these conditions are checked directly during transaction validation.

In contrast, Nervos' CKB-VM is more akin to a traditional VM, executing the rules associated with cells in a controlled environment.

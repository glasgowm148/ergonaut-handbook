---
title: ErgoScript
description: The underlying smart contract language of Ergo.
published: false
date: 2022-09-20T16:12:18.634Z
tags: programming, coding, developers, scala
editor: markdown
dateCreated: 2022-09-20T15:09:13.590Z
---

# ErgoScript
ErgoScript is a powerful and protocol-friendly scripting language for cryptocurrencies. Programs in ErgoScript are used to specify the conditions under which currency can be spent. The language supports a type of non-interactive zero-knowledge proofs called [Sigma (Σ) protocols](https://ergonaut.space/en/Glossary/sigma-protocols) and is flexible enough to allow for: ring-signatures, multi signatures, multiple currencies, [atomic swaps](/en/Glossary/Atomic-Swaps), self-replicating scripts, and long-term computation.

**ErgoScript is a super-simple subset of Scala.** It is a top-level language translated into a low-level language called ErgoTree, which is translated during execution into cryptographic protocol. 

Ergo's support for sigma-protocols (aka generalized Schnorr proofs) is truly unique. As building bricks for composable statements, Ergo supports Schnorr protocols and proof-of-Diffie-Hellman-tuples, but more can be added via soft-forks


## Key Concepts

- Ergo is considered an *extended-UTXO model*, supporting advanced financial contracts similar to those in Ethereum's account-based model
- Since Ergo is UTXO based, therefore ErgoScript has many UTXO-specific constructs such as: 
  - `Box`, `INPUTS`, `OUTPUTS`
  - A complete list is available [here](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/LangSpec.md)
- A `Box` is essentially a UTXO and consists of up to ten registers for storing data. Similar to Bitcoin, a transaction spends one or more existing boxes (denoted using the `INPUTS` array), and creates one or more new boxes (denoted using the `OUTPUTS` array)
- ErgoScript's syntax is a subset of Scala's. However, knowledge of Scala is not necessary to learn ErgoScript because the amount of Scala needed to write ErgoScript is small e.g. `val`
- Note that arrays in Scala are accessed using round parentheses, not square brackets like in Java or Python. Thus, `OUTPUTS(0)` refers to the first element of the `OUTPUTS` array
- Unlike Scala, ErgoScript does not support the `var` keyword, and thus everything is immutable
- The scripting language in itself is non-Turing complete, but applications can be made to be Turing complete as demonstrated in [this peer-reviewed paper](https://arxiv.org/pdf/1806.10116v1.pdf).


## Resources

### Tutorials 

- [Learn ErgoScript By Example Via The Ergo Playground with Robert Kornacki (Video)](https://www.youtube.com/watch?v=8l2v1asHgyA)
- [ErgoScript by Example Repository](https://github.com/ergoplatform/ergoscript-by-example)
- [Testing Ergo Contracts Off-chain](https://github.com/anon-real/contract-testing)
- [Deco-Education/ErgoScript-Developer-Course](https://github.com/DeCo-Education/ErgoScript-Developer-Course)
- [Deco Education: 2022 Script Class](https://www.youtube.com/watch?v=qR0_k7VH6KI&list=PLopsKGshj0B4DfFnS-pvriZhba050eaXu)
### Advanced Tutorials

- [Advanced ErgoScript Tutorial](https://ergoplatform.org/docs/AdvancedErgoScriptTutorial.pdf)
- [ErgoScript tutorial](https://ergoplatform.org/docs/ErgoScript.pdf)


### Explanations

- [ErgoScript Design patterns](https://www.ergoforum.org/t/ergoscript-design-patterns/222)
- [SigmaState Protocols](https://docs.ergoplatform.com/sigmastate_protocols.pdf)

### References

- [ErgoScript Language Spec](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/LangSpec.md)
- [ErgoScript](https://ergoplatform.org/docs/ErgoScript.pdf) 
- [ErgoTree](https://ergoplatform.org/docs/ErgoTree.pdf)
- [High Level Design Patterns In Extended UTXO Systems](https://github.com/Emurgo/Emurgo-Research/blob/master/smart-contracts/High%20Level%20Design%20Patterns%20In%20Extended%20UTXO%20Systems.md)

### Examples

- [ErgoPad Staking Contracts](https://github.com/ergo-pad/ergopad/blob/staking-contracts/backend/app/contracts/staking.md)
- [GetBlok.io Smart Pools](https://github.com/GetBlok-io/ergo-smartpooling-contracts)


### Visual

- [FlowCards](flowcards.md) | A Declarative Framework for Development of Ergo dApps (Also see [flowcardLib](https://github.com/lucagdangelo/flowcardLib))
- [flowcardLib: Ergo FlowCard library for diagrams.net](https://github.com/lucagdangelo/flowcardLib)
- [ergo-castanet](https://github.com/iandebeer/ergo-castanet)

### Bookmarks


- Compile ErgoScript directly in your browser with [ErgoScript Playground](https://wallet.plutomonkey.com/p2s/)
- [Kiosk](/dev/stack/kiosk) lets anyone play with ErgoScript using a basic web-based UI
- [ergoscript-compiler](https://github.com/ergoplatform/ergoscript-compiler)


---
title: Ergo vs KAS
description: 
published: true
date: 2023-08-07T09:39:17.469Z
tags: 
editor: markdown
dateCreated: 2023-08-07T09:26:17.272Z
---

# Ergo vs Kaspa

Ergo and Kaspa are two cryptocurrencies that have been gaining attention in the crypto space. Both have their unique features and technologies, but when it comes to well-researched, known methods, and tried and tested principles, Ergo stands out as the superior choice.

Ergo is a decentralized blockchain platform designed to provide an efficient, secure, and easy way to implement financial contracts. It uses a unique consensus algorithm called Autolykos, a Proof-of-Work (PoW) algorithm designed to be ASIC-resistant. This makes it more decentralized and fairer than other PoW cryptocurrencies. Ergo also features smart contract capabilities, with its own language called ErgoScript, which is a powerful and protocol-friendly scripting language for cryptocurrencies. This makes it possible to create complex financial contracts on the Ergo platform. Furthermore, Ergo emphasizes privacy, with features such as "ring signatures" and "zero-knowledge proofs" to ensure transactions can be private.

In 2023, Ergo continued to make strides in its development. The Ergo Summit celebrated progress within the ecosystem. EIP-27, a proposal to adjust the emission schedule of ERG to extend the mining rewards beyond the original eight-year schedule, marked an important milestone for the Ergo network and ecosystem. 

On the other hand, Kaspa, which uses the ghostDAG protocol, is still experimental and may not be the best place for robust financial contracts. As noted by kushti khushi, a core developer of Ergo, after examining Kaspa's core code, he expressed doubts about the introduction of smart contracts on the Kaspa platform due to its complex input signing with different sighash options taken from Bitcoin. He also questioned the use of muhash for state authentication in Kaspa, and why an incremental hash was used instead of an authenticated dictionary. The presence of a directed acyclic graph (DAG) in Kaspa could lead to a verification dilemma, which might not have been adequately addressed in the ghostDAG paper and its continuations.

In 2023, Kaspa was still in the development phase, with a white paper scheduled for release that would combine Kaspa's past research and current goals into a cohesive document. Kaspa also achieved a milestone by reaching 10 Blocks Per Second (BPS) on its testnet, setting a new standard in the world of cryptography. However, these developments are still in the experimental stage, and the platform's suitability for robust financial contracts remains to be seen.

In conclusion, while Kaspa's ghostDAG protocol presents an interesting and innovative approach to blockchain technology, its experimental nature and potential issues suggest that it may not be the most reliable platform for financial contracts. On the other hand, Ergo, with its well-researched and tested principles, offers a more solid and reliable platform for such purposes. As always, potential investors should conduct their own research and consider their risk tolerance before investing in any cryptocurrency.
| Feature | Ergo (ERG) | Kaspa (KSP) |
|---------|------------|-------------|
| **Consensus Mechanism** | Autolykos (Proof-of-Work) | ghostDAG protocol |
| **Smart Contracts** | Yes, with [ErgoScript](https://docs.ergoplatform.com/dev/scs/ergoscript/) | No |
| **Privacy Features** | Yes, includes ring signatures and zero-knowledge proofs | No |
| **Scalability** | Aims to solve [scalability with the power of eUTXO, NiPoPoWs and other novel features](https://docs.ergoplatform.com/dev/protocol/scaling/) | Aims to solve scalability issues with ghostDAG protocol |
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
>
> Which is solving verification dilemma for miners at least but a very different beast from blockchains we know
>
> But Kaspa is so extreme from initial investigation
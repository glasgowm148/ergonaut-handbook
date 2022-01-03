---
title: Overview
description: Community gathered resources for the Ergo blockchain
published: true
date: 2022-01-03T11:08:29.636Z
tags: 
editor: markdown
dateCreated: 2021-02-24T07:55:49.194Z
---

> ergonaut.space is a community driven space where anyone can contribute. Contact @glasgowm/unomie/sigmanaut\_ on telegram/Discord/reddit to have a new regional language section added.
{.is-success}


## The Next Generation of Blockchain

Ergo is a Layer 1 proof of work blockchain that provides a platform for developers to build trustless financial contracts and enables true peer to peer, decentralised, grassroots finance.

Ergo has prioritised useful features without compromising security with a research-driven but practical development model. 

*Ergo*, **a resilient platform for contractual money**



-   See the [Ergo Wiki](https://github.com/ergoplatform/ergo/wiki) on GitHub

> *“It's one of the most revolutionary cryptocurrencies ever built. Got so many crazy ideas like sigma protocols and pruning the blockchain and roller chains. All this crazy stuff. Even has a proof of no premine. So really a technological marvel in many respects, and it reflects about 8 years of knowledge that Alex has amassed as both a researcher and a developer. Super concise code and it blows my mind that the market cap is where it's at. It should be a top 10 coin or top 15 coin"* — Charles Hoskinson



> Research-led but real-world focused

Ergo Platform's native token, ERG, is used to pay all transaction fees for transfers and smart contract execution. Storage fees are also charged on dormant accounts, providing ongoing incentives for miners even after block rewards end. This new economic model ensures a sustainable network. ERG functions as the core token and will be used for different dApps collateral like stablecoin and many other applications. Off-the-peg use of ring and threshold signatures powers non-custodial and non-interactive dApps like ErgoMixer for both ERG and custom tokens.

Custom tokens are first-class citizen tokens in Ergo; there is also atomic exchange built for them in the core. Custom tokens can be distributed to miners and other ecosystem stakeholders, using logically defined smart contracts, including built-in PoW-style emission schedules.

Ergo is designed from scratch, including its POW algorithm, Autolykos v2, memory-hard, GPU friendly, and based on fairness. Ergo team believes that network should adapt to changing environment without the intervention of trusted parties, so it has an on-chain miner voting protocol that allows gradual changes in a large number of parameters, including maximum block size, storage fee factor, and more, for more fundamental changes Ergo is trying to follow a soft-fork ability approach if an overwhelming majority of the network accepts a new feature, it is then activated, however, old nodes which do not upgrade will continue to operate normally and skip over this feature validation.

Ergo is designed to be a self-amendable protocol that allows to absorb new ideas and improve itself in a decentralized manner.


## Powerful but safe

In our different experiences of working with blockchain platforms, we've learned that conventional Turing-complete smart contracts may be powerful, but they can be risky. Implementing complex computational tasks on the blockchain can have unintended consequences. Network conditions, bugs and code exploits can mean it's impossible to know how expensive it is to execute software – or whether that code will run as intended at all. That can lead to security vulnerabilities and faulty dApps.

Ergo's smart contracts allow us to execute wide-ranging tasks, but we always know in advance how much the code will cost and whether it will run successfully. Meanwhile, we can still write Turing-complete scripts by iterating processes across multiple blocks. That means Ergo can support versatile dApps that run predictably, with known costs, and don't have any of the dangers of unrestricted functionality.

## Intelligent but straightforward

Sigma protocols are the foundation of Ergo's smart contracts. They allow for a class of efficient zero-knowledge protocols that enable us to implement tasks that would otherwise be either impossible or risky and expensive.

For example, Sigma protocols let us implement ring and threshold signatures out of the box. Let's say you want to create a 'ring spending contract', where either of us can make a transaction from the same address, but we don't want anyone else to know which one of us is spending the funds. That's not possible with Bitcoin. While Ethereum can do it with Ethereum, it would be expensive and complicated – especially with a ring size of 10 or 20 members, required for robust privacy.

With Ergo, this kind of application can be created quickly, thanks to the integration of Sigma protocols in the core. This enables self-sovereign application-level privacy: trustless scripts that can be used to access mixers or other functionality without any third parties required.

## Secure but accessible

Each script is applied to an unspent output. We have drawn this feature from the Bitcoin protocol, which uses UTXOs or the 'coin' model rather than an 'account' model like Ethereum's. We consider this a more secure approach since boxes are immutable, as well as being more flexible.

Ergo's blockchain uses the Autolykos algorithm for consensus, which is a variant of Equihash and offers better ASIC resistance and a degree of pool resistance. This enables better decentralization, avoiding large pools that can collude or be coerced to attack the network. At the same time, we recognize that ordinary users who do not run a full node should enjoy the same security benefits as miners. Ergo's non-interactive proof-of-proof-of-work (NiPoPoW) allows anyone to make and verify transactions with complete confidence, without needing the storage, bandwidth and time required to download the full blockchain. As little as 1 MB of data is needed – meaning any device can be used.

> In regards to security, we always tried to use the most straightforward and well-studied approach; otherwise, to cover a new direction with a published paper and a lot of testing. We considered some things seriously other projects are fixing after attacks only, e.g. spammy contracts (causing "verifier's dilemma").

## Deflationary but economically sustainable

Like many other features in Ergo, the network's economic model is based on Bitcoin's approach. We believe that digital scarcity is essential for underpinning value and capped coin supply under 100 million ERG. Unlike Bitcoin, the block rewards decrease steadily after the first two years, with no long tail of emission. Block rewards start at 75 ERG, and over eight years will fall to zero, after which total supply will be fixed.

At this point, in addition to transaction fees, miners will also benefit from storage rent fees charged on boxes (UTXOs) that have not moved their coins for four years or more. There are at least two advantages to this approach. Firstly, it gives miners an additional source of revenues once block rewards end. Since the network's security depends on the hash rate and miner participation, this is a significant incentive to provide. Secondly, it has the effect of recycling lost coins (and dust) back into the Ergo economy. Research suggests that up to 4 million BTC have been permanently removed from circulation due to lost private keys. Ergo's storage fees will slowly reclaim these for productive purposes, while users who want to hold coins for the long term can avoid being charged simply by moving their funds.

## PoW mined but protocol-funded

There is a difficult balance between ensuring a project is adequately funded and potentially disadvantaging later users if a large proportion of tokens is pre-mined or reserved in an ICO. We have chosen a strategy that has proven successful for other cryptocurrencies, whereby a percentage of tokens from each block reward is allocated for development and marketing.

In Ergo's case, these Foundation tokens are managed by a smart contract built into the protocol. 10% of each block reward for the first two years, or 7.5 ERG per block, are allocated to the Treasury, with the remaining 67.5 ERG going to miners. As block rewards begin to reduce after two years, the Foundation will continue to receive rewards over 67.5 ERG, with the Treasury allocation dropping to zero after 2.5 years.

## Consensus-led but readily adaptable

Ergo is designed and implemented by a team of experienced developers and researchers who hold publications and PhDs in cryptography, compiler theory, blockchain technology, and cryptographic e-cash. The team also has a solid background in core development with such cryptocurrencies and blockchain frameworks as Nxt, Scorex and Waves.

We are also supported by community developers, who may work on a volunteer basis or receive grants from the Foundation to implement useful features and dApps. For example, ErgoMix, a decentralized mixing service based on Sigma protocols, was built by a third-party developer from the Ergo community, and Ergo's decentralized exchange is also being developed on this basis.

## Community-driven but Agile

Ergo is designed and implemented by a team of experienced developers and researchers who hold publications and PhDs in cryptography, compiler theory, blockchain technology, and cryptographic e-cash. The team also has a solid background in core development with such cryptocurrencies and blockchain frameworks as Nxt, Scorex and Waves.

Long‐term survivability and self‐amenability are what give Ergo its resiliency. Constant and stable community-driven growth: there was no ICO / VC support and **no pre-mine**

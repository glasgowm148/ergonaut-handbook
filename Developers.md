---
title: Developers
description: 
published: true
date: 2021-04-10T13:29:58.267Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:19:45.758Z
---

> Ergo enables new models of financial interaction, underpinned by smart contracts built on flexible and powerful Sigma protocols but easily accessible to developers.
{.is-info}




# Overview


- See the currently deployed dApps on [sigmaverse.io](https://sigmaverse.io/)
- [Ergo dApp Ecosystem Development - ergoforum](https://www.ergoforum.org/t/what-apps-can-you-do-on-ergo/819)


**Services**
- Mainnet explorer: https://explorer.ergoplatform.com/
- Testnet explorer: https://testnet.ergoplatform.com/
# Languages

## ErgoScript
Learn [Ergoscript by reading example smart contracts](https://github.com/ergoplatform/ergoscript-by-example) powered by the Ergo Playground.

Each contract example includes a `Ergo Playground` link which allows you to instantly edit and run the smart contract code inside of your browser.

If you ever need clarity about how specific types/functions/operators in ErgoScript work, please reference the [ErgoScript Language Description](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/LangSpec.md).

For an overarching summary of how everything in this repo works, please reference the video [ErgoScript By Example & Ergo Playground Introductory Video](https://www.youtube.com/watch?v=8l2v1asHgyA)

 - [ErgoScript by Example](https://github.com/ergoplatform/ergoscript-by-example) - repository with ErgoScript examples you can play with in Ergo Playground 
 - [Ergo notary](https://github.com/sininen-taivas/ergo-notary) - simple command-line tool to certificate files on the Ergo blockchain. 
 See also [forum topic](https://www.ergoforum.org/t/ergo-notary-command-line-tool/75) on a particular example
 - [Miner rewards script](https://github.com/lorien/ergotools) Simple command-line tool to find miner rewards not spent and form withdrawing transaction requests for them
 - [A Quick Primer on ErgoScript](https://github.com/ergoplatform/ergo/wiki/ErgoScript-Overview) Learn the basics of ErgoScript quickly and create your first contract
 - [ErgoScript Design patterns](https://www.ergoforum.org/t/ergoscript-design-patterns/222)

 
 you can do that with node API and also ErgoScript to P2S (pay-to-script) address  compiler, e.g. `https://wallet.plutomonkey.com/p2s` . For example, you want to create a coin anyone can spend. Then create and compile to P2S address the following script:

`https://wallet.plutomonkey.com/p2s/?source=ewogIHRydWUKfQ==`

And then use `http://127.0.0.1:9053/swagger#/utils/AddressToRaw` API call to get "raw" representation of the address, so script bytes in case of P2S (the result is the same as `ErgoTreeSerializer.DefaultSerializer.serializeErgoTree(script)`) . For the example script the result would be
```
{
  "raw": "10010101d17300"
}
```

## Rust

[Sigma-rust](https://github.com/ergoplatform/sigma-rust) - implementation of ErgoScript cryptocurrency scripting language. To get better understanding on how to use it in your project check out how its being used in the following projects:

- [Ergo Headless dApp Framework](https://github.com/Emurgo/ergo-headless-dapp-framework);
- [Ergo Node Interface Library](https://github.com/Emurgo/ergo-node-interface);
- [Oracle Core](https://github.com/ergoplatform/oracle-core);
- [AgeUSD Stablecoin Protocol](https://github.com/Emurgo/age-usd);
- [Yoroi wallet](https://github.com/Emurgo/yoroi-frontend) (WASM bindings);
- [Ergo Desktop Wallet](https://github.com/ErgoWallet/ergowallet-desktop) (WASM bindings);

> New developer? A list of "*good first*" issues for Sigma-Rust is [available on GitHub](https://github.com/ergoplatform/sigma-rust/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22 ) - @greenhat on [Discord](https://discord.gg/Q86PNMwRsu) is ready to assist anyone who is interested.
{.is-info}

## Scala

- Smart contract language: https://github.com/ScorexFoundation/sigmastate-interpreter
- Basic cryptography library: https://github.com/input-output-hk/scrypto

## JS

- Typescrypt library with support of tokens and complex transactions: https://github.com/coinbarn/ergo-ts
- Basic transaction operations: https://github.com/ergoplatform/ergo-js

# Libaries

- Ergo-Bootstrap: easy to use tool with cluster deployments for dApp development


**Test vectors:**
- Ergo transaction serialization: https://git.io/fjqwX
- Signature scheme: https://git.io/fjqwH


## Appkit

[Appkit](https://github.com/ergoplatform/ergo-appkit): A Library for Polyglot Development of Ergo Applications

The Appkit library is based on GraalVM - a novel next generation approach to implement software which is reusable across several programming languages and execution environments.

Appkit has idiomatic Java API and is written in Java/Scala. It is a thin wrapper around core components provided by ErgoScript interpreter and Ergo protocol implementations which are written in Scala.

Using Appkit Ergo applications can be written in one of the languages supported by GraalVM (i.e. Java, JavaScript, C/C++, Python, Ruby, R) and using this library applications can communicate with Ergo nodes via unified API and programming model provided by Appkit. In addition Appkit based Ergo applications can be compiled into native code using native-image ahead of time compiler and then executed without Java VM with very fast startup time and lower runtime memory overhead compared to a Java VM.

## ErgoDEX sdk

https://github.com/ergoplatform/ergo-dex-sdk-js



# Frameworks
- [FlowCards: A Declarative Framework for Development of Ergo dApps](https://ergoplatform.org/en/blog/2020_04_29_flow_cards/)
## Scorex 
 The modular blockchain framework
https://github.com/scorexfoundation/scorex


## Sigmastate-Interpreter

Interpreter for a family of Sigma-State authentication languages, [a list of good first issues is available on Github](https://github.com/ScorexFoundation/sigmastate-interpreter/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22)

Once implemented, it will be used in Explorer, Playground and probably other tools.


# Misc

- [Multi-Stage Contracts in the UTXO Model: Delivery by Alexander Chepurnoy & Amitabh Saxena](https://www.youtube.com/watch?v=g3FlM_WOwBU)
- [Non-Interactive Proofs of Proof-of-Work](https://eprint.iacr.org/2017/963.pdf)

## API

- [Node API](https://git.io/fjqwb)
- [Explorer API](https://git.io/fjqwN)

## Tools
 - [Sigma-Rust](https://github.com/ergoplatform/sigma-rust/) - Alternative and simple implementation of ErgoTree interpreter and transaction building tools
 - [Ergo Utilities](https://github.com/robkorn/ergo-utilities-rust/) - General utilities to make writing off-chain Ergo code in Rust simpler 
 - [Ergo Appkit (Polyglot library)](https://github.com/aslesarenko/ergo-appkit) - Appkit: A Library for Polyglot Development of Ergo Applications using [GraalVM](https://www.graalvm.org/)
 - [ergo-ts (TypeScript)](https://github.com/coinbarn/ergo-ts)
 - [ergo-js (JavaScript)](https://github.com/ergoplatform/ergo-js) 
 - [Kiosk](https://github.com/scalahub/Kiosk) - interface to Ergo node with additional features for a developer. See this [forum post](https://www.ergoforum.org/t/ergoscript-playground-using-kiosk/96) about particular example 
 - [Appkit Examples](https://github.com/aslesarenko/ergo-appkit-examples) - Examples of using Ergo Appkit for Polyglot Development of Ergo Applications
 - [ErgoTool](https://github.com/aslesarenko/ergo-tool) - A Command Line Interface for Ergo based on Appkit and [GraalVM](https://www.graalvm.org/)
 - [Ergo P2S Playground](https://wallet.plutomonkey.com/p2s/?source=dHJ1ZQ==) - A web-based tool to quickly get the address corresponding to some script  
[Video tutorial #2](https://www.youtube.com/watch?v=DgztoNDFG8U) 
 - [Oracle Core](https://github.com/ergoplatform/oracle-core) - Run your oracle pools!

## dApps
  - [ErgoMixer](https://github.com/ergoMixer/ergoMixBack) - Non-interactive and non-custodial mixer! [Video tutorial #1](https://www.youtube.com/watch?v=03_2HH82Plw),
- [Ergo Auctions House](http://ergoauctions.org/#/auction/active) - Buy and sell collectible tokens and not only! [Source code](https://github.com/anon-real/ErgoAuctionHouse)
 - ZK Treasury: [Server](https://github.com/anon-real/DistributedSigsServer) and [Client](https://github.com/anon-real/DistributedSigsClient) - a tool for joint spendings with on-chain privacy 


## CLI

 - [Ergo oracles](https://github.com/sininen-taivas/ergo-oracle) - simple command-line tool to launch oracles. Inbuilt implementations for USD/ERG, EUR/ERG, BTC/ERG, AUG/ERG (gold) prices delivery. See also a [forum topic with example](https://www.ergoforum.org/t/erg-usd-oracle-on-top-of-ergo/119)
 - [Ergo Crowdfunding CLI](https://github.com/robkorn/ergo-crowdfunding-cli) Command-line tool which enables participating and interacting with crowdfunding campaigns on Ergo 

# Documents

**Manuals**

- Full node set-up: https://git.io/fjqwx
- Start mining: https://git.io/fjqwp

- White paper: https://docs.ergoplatform.com/whitepaper.pdf
- Yellow paper (in progress): https://docs.ergoplatform.com/YellowPaper.pdf
- Short overview: https://docs.ergoplatform.com/teaser.pdf
- ErgoScript tutorial: https://docs.ergoplatform.com/ErgoScript.pdf
- ErgoScript advanced tutorial: https://docs.ergoplatform.com/sigmastate_protocols.pdf
- Autolykos PoW scheme specification: https://docs.ergoplatform.com/ErgoPow.pdf

**Sources**:
- Main repository: https://github.com/ergoplatform/ergo

# ZK Treasury

## Proposed Nautilus ZK Treasury

This basic concept is to create a visual programming toolkit to assist developers in learning and developing contracts in the EUTXO model. 

This toolkit will initially be built on top of Ergo Playground.  

The goal is to take advantage of the free composability offered by EUTXO. Create an open source library of visual, composable tools to onboard new developers. 

The “long term” goal is to create a headless central management system for developers, and a front-end UI focused central management system for basic users that are both interoperable with this visual programming toolkit. 

The name Nautilus is inspired by the Submarine in Jules Verne 20,000 Leagues Under the Sea. Nautilus is described by Verne as "a masterpiece containing masterpieces", which was built in secrecy, sourcing parts from unnamed sources and roams the seas beyond the reach of land-based governments.





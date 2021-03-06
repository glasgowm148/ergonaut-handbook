---
title: Developers
description: 
published: true
date: 2021-05-05T09:36:51.026Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:19:45.758Z
---

> This site is a community resource website, ergonauts are encouraged to create an account and add to the site. the site is backed up and available to use on [Github](https://github.com/glasgowm148/ergonaut-handbook). Submit pull requests to update this (and other) pages!
{.is-info}

# Getting Started
The Ergo ecosystem is quickly growing with new design patterns, tools, dApps, and more every single month. This is an exciting point in time for developers to jump in and get started.

That said, while building dApps on top of Ergo, vital infrastructure components to develop and run your dApp might be intimidating to set up for someone who is unfamiliar with the existing tooling. Between an Ergo full node, explorer back end, explorer front end, logging, and metrics, it can become quite overwhelming for a nascent dApp developer entering into the ecosystem.

For this reason, we are introducing [ergo-bootstrap](https://github.com/ergoplatform/ergo-bootstrap), an easy-to-use tool that enables quick and clean Ergo blockchain cluster deployments which supports a variety of useful infrastructure components you will need on your path of dApp development. This was developed by Marek of Five Binaries thanks to a grant given by the Ergo Foundation and their latest push to empower the ecosystem via funding key projects.

Ergo bootstrap tool, build on top of ergo-nix, will help you to quickly deploy an Ergo blockchain cluster with a handful of useful tools you might need to start developing your dApps.

Read more on the blog - [Ergo Bootstrap, Streamlining Ergo dApp Infrastructure With One Simple Tool](https://ergoplatform.org/en/blog/2020-12-11-ergo-bootstrap-streamlining-ergo-dapp-infrastructure-with-one-simple-tool/)

You can see the currently deployed dApps on [sigmaverse.io](https://sigmaverse.io/), and this recent post on the forum on [Ergo dApp Ecosystem Development - ergoforum](https://www.ergoforum.org/t/what-apps-can-you-do-on-ergo/819) gives some indication to where development is needed. 

## Hackathon

We are thinking about organizing a hackathon, likely in May. The topic would be "**Completing the Basics**", so improving basic infrastructure needed for building the DApps, (also, to profit from them) 

The following topics will likely be covered

* Improvements to ErgoScript (not all the ErgoTree features are projected into it)
* Improvements to [Ergo AppKit](https://github.com/ergoplatform/ergo-appkit) (basic library for constructing transactions and building offchain logic on top of for Java and JVM languages) 
* Improvements to Ergo Node Interface and - [Ergo Headless dApp Framework](https://github.com/Emurgo/ergo-headless-dapp-framework) (basic library for constructing transactions and building offchain logic with Rust)
* [Ergo Crowdfunding](https://github.com/robkorn/ergo-crowdfunding-cli) apps/UI 
* Visual tool for constructing multi-signatures (could be a good first step for visual tools to construct more complex scripts)
* Tokenization schemes
* Tools for NFTs
* Applications for data notarization and names registration
* Stealth addresses pool implementation
* Applications on top of mixer API 
* More data connectors for the oracle pools
* Private swaps with other chains on Schnorr signature (Bitcoin Cash, Litecoin (?), Komodo (?))

Everyone participating will be rewarded for delivering anything that progresses the current state.




# Languages

## ErgoScript
Learn [Ergoscript by reading example smart contracts](https://github.com/ergoplatform/ergoscript-by-example) powered by the Ergo Playground. Each contract example includes a `Ergo Playground` link which allows you to instantly edit and run the smart contract code inside of your browser.

- If you ever need clarity about how specific types/functions/operators in ErgoScript work, please reference the [ErgoScript Language Description](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/LangSpec.md).
- For an overarching summary, please reference this [video](https://www.youtube.com/watch?v=8l2v1asHgyA)
 - [A Quick Primer on ErgoScript](https://github.com/ergoplatform/ergo/wiki/ErgoScript-Overview) Learn the basics of ErgoScript quickly and create your first contract
 - [ErgoScript Design patterns](https://www.ergoforum.org/t/ergoscript-design-patterns/222)




## Rust
> A list of "*good first*" issues for Sigma-Rust is [available on GitHub](https://github.com/ergoplatform/sigma-rust/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22 ) - @greenhat on [Discord](https://discord.gg/Q86PNMwRsu) is ready to assist anyone who is interested.
{.is-info}

[Sigma-rust](https://github.com/ergoplatform/sigma-rust) - implementation of ErgoScript cryptocurrency scripting language. To get better understanding on how to use it in your project check out how its being used in the following projects:

- [Ergo Headless dApp Framework](https://github.com/Emurgo/ergo-headless-dapp-framework);
- [Ergo Node Interface Library](https://github.com/Emurgo/ergo-node-interface);
- [Oracle Core](https://github.com/ergoplatform/oracle-core);
- [AgeUSD Stablecoin Protocol](https://github.com/Emurgo/age-usd);
- [Yoroi wallet](https://github.com/Emurgo/yoroi-frontend) (WASM bindings);
- [Ergo Desktop Wallet](https://github.com/ErgoWallet/ergowallet-desktop) (WASM bindings);
- [Ergo Utilities](https://github.com/robkorn/ergo-utilities-rust/) - General utilities to make writing off-chain Ergo code in Rust simpler 


## Scala

- Smart contract language: https://github.com/ScorexFoundation/sigmastate-interpreter
- Basic cryptography library: https://github.com/input-output-hk/scrypto

## JS/TS

 - [ergo-ts (TypeScript)](https://github.com/coinbarn/ergo-ts) with support of tokens and complex transactions
 - [ergo-js (JavaScript)](https://github.com/ergoplatform/ergo-js) with basic transaction operations
 - [Ergo JS Template](https://github.com/anon-real/ergo-js-template)





# Frameworks

## Sigmastate-Interpreter

Interpreter for a family of Sigma-State authentication languages, [a list of good first issues is available on Github](https://github.com/ScorexFoundation/sigmastate-interpreter/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22)

## Oracle Core
The oracle core is the off-chain component that oracles who are part of an oracle pool run. This oracle core provides a HTTP API interface for reading the current protocol state & another for submitting datapoints. Once a datapoint is submited, the oracle core will automatically generate the required tx and post it as well as any other actions required for the protocol to run. This thereby allows the oracle to participate in the oracle pool protocol without any extra effort for the oracle operator.
- [Oracle Core](https://github.com/ergoplatform/oracle-core) - Run your oracle pools!

## Scorex 

- [ScoreX](https://github.com/scorexfoundation/scorex), The modular blockchain framework

## Tools

 - [Kiosk](https://github.com/scalahub/Kiosk) - interface to Ergo node with additional features for developers. See this [forum post](https://www.ergoforum.org/t/ergoscript-playground-using-kiosk/96) for examples. 
 - [Ergo P2S Playground](https://wallet.plutomonkey.com/p2s/?source=dHJ1ZQ==) - A web-based tool to quickly get the address that corresponding to a script - [Video tutorial #2](https://www.youtube.com/watch?v=DgztoNDFG8U) 
 - [ergo-dex-sdk-js](https://github.com/ergoplatform/ergo-dex-sdk-js)

### Appkit

 - [Ergo Appkit (Polyglot library)](https://github.com/aslesarenko/ergo-appkit) - Appkit: A Library for Polyglot Development of Ergo Applications using either [GraalVM](https://www.graalvm.org/) or stock Java 1.7 and above. Read the [introduction](https://ergoplatform.org/en/blog/2019_12_03_top5/).
  - [Appkit Examples](https://github.com/aslesarenko/ergo-appkit-examples) - Examples of using Ergo Appkit for Polyglot Development of Ergo Applications
  - [Ergo Android](https://github.com/aslesarenko/ergo-android) - Example Android application which demonstrates how Ergo Appkit can be used to develop Ergo applications running on Android.

Appkit has idiomatic Java API and is written in Java/Scala. It is a thin wrapper around core components provided by ErgoScript interpreter and Ergo protocol implementations which are written in Scala. It is [published](https://mvnrepository.com/artifact/org.ergoplatform/ergo-appkit) on maven repository and cross compiled to both Java 7 and Java 8+ jars.

The Appkit library is compatible with GraalVM - a novel next generation approach to implement software which is reusable across several programming languages and execution environments. For example if Node.js application is run on GraalVM, then it can use Appkit to interact with Ergo Blockchain.


Using Appkit Ergo applications can be written in one of the languages supported by GraalVM (i.e. Java, JavaScript, C/C++, Python, Ruby, R) and using this library applications can communicate with Ergo nodes via unified API and programming model provided by Appkit. In addition Appkit based Ergo applications can be compiled into native code using native-image ahead of time compiler and then executed without Java VM with very fast startup time and lower runtime memory overhead compared to a Java VM. This is attractive option for high-performance low-latency microservices. 

In addition Appkit is compatible with Android and can be used from Android applications. 

 - [ErgoTool](https://github.com/aslesarenko/ergo-tool) - A Command Line Interface for Ergo based on Appkit and [GraalVM](https://www.graalvm.org/) native-image. Read the [introduction and overview](https://ergoplatform.org/en/blog/2019_12_31_ergo_tool/).
 

# Misc

- [Main repository](https://github.com/ergoplatform/ergo)
- [Multi-Stage Contracts in the UTXO Model: Delivery by Alexander Chepurnoy & Amitabh Saxena](https://www.youtube.com/watch?v=g3FlM_WOwBU)
- [Non-Interactive Proofs of Proof-of-Work](https://eprint.iacr.org/2017/963.pdf)


##  Ergo Improvement Proposals

Ergo Improvement Proposals (EIPs) specify and/or describe standards for the Ergo Platform, including core protocol specifications, client APIs, dApp/contract standards, and other such things.

Please check out existing EIPs, such as [EIP-1](eip-0001.md), to understand the general expectation of how EIPs are supposed to be formatted.

| Number | Title |
| ---  | ---  |
| [EIP-0001](eip-0001.md) | UTXO-Set Scanning Wallet API |
| [EIP-0002](eip-0002.md) | Ergo Grant Program | 
| [EIP-0003](eip-0003.md) | BIP-44 Standard For Ergo Platform | 
| [EIP-0004](eip-0004.md) | Assets Standard | 
| [EIP-0005](eip-0005.md) | Contract Template | 
| [EIP-0006](eip-0006.md) | Informal Smart Contract Protocol Specification Format | 



**Test vectors:**
- [Ergo transaction serialization](https://git.io/fjqwX)
- [Signature scheme](https://git.io/fjqwH)



## Services
- [Mainnet explorer](https://explorer.ergoplatform.com/)
- [Testnet explorer](https://testnet.ergoplatform.com/)
- [Node API](https://git.io/fjqwb)
- [Explorer API](https://git.io/fjqwN)
- [API Docs](https://api.ergoplatform.com/api/v1/docs/)



## dApps
  - [ErgoMixer](https://github.com/ergoMixer/ergoMixBack) - Non-interactive and non-custodial mixer! [Video tutorial #1](https://www.youtube.com/watch?v=03_2HH82Plw),
- [Ergo Auctions House](http://ergoauctions.org/#/auction/active) - Buy and sell collectible tokens and not only! [Source code](https://github.com/anon-real/ErgoAuctionHouse)
 - ZK Treasury: [Server](https://github.com/anon-real/DistributedSigsServer) and [Client](https://github.com/anon-real/DistributedSigsClient) - a tool for joint spendings with on-chain privacy 


## CLI
 - [Ergo notary](https://github.com/sininen-taivas/ergo-notary) - simple command-line tool to certificate files on the Ergo blockchain. See also [forum topic](https://www.ergoforum.org/t/ergo-notary-command-line-tool/75) on a particular example
 - [Miner rewards script](https://github.com/lorien/ergotools) Simple command-line tool to find miner rewards not spent and form withdrawing transaction requests for them
 - [Ergo oracles](https://github.com/sininen-taivas/ergo-oracle) - simple command-line tool to launch oracles. Inbuilt implementations for USD/ERG, EUR/ERG, BTC/ERG, AUG/ERG (gold) prices delivery. See also a [forum topic with example](https://www.ergoforum.org/t/erg-usd-oracle-on-top-of-ergo/119)
 - [Ergo Crowdfunding CLI](https://github.com/robkorn/ergo-crowdfunding-cli) Command-line tool which enables participating and interacting with crowdfunding campaigns on Ergo 
 - [ErgoTool](https://github.com/aslesarenko/ergo-tool) - A Command Line Interface for Ergo based on Appkit and [GraalVM](https://www.graalvm.org/)


# Documentation

- [FlowCards: A Declarative Framework for Development of Ergo dApps](https://ergoplatform.org/en/blog/2020_04_29_flow_cards/)
- [Full node set-up](https://git.io/fjqwx)
- [Start mining](https://git.io/fjqwp)
- [White paper]( https://docs.ergoplatform.com/whitepaper.pdf)
- [Yellow paper (in progress)]( https://docs.ergoplatform.com/YellowPaper.pdf)
- [Short overview]( https://docs.ergoplatform.com/teaser.pdf)
- [ErgoScript Language Description](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/LangSpec.md) 
- [ErgoScript tutorial]( https://docs.ergoplatform.com/ErgoScript.pdf)
- [ErgoScript advanced tutorial]( https://docs.ergoplatform.com/sigmastate_protocols.pdf)
- [ErgoTree specification](https://ergoplatform.org/docs/ErgoTree.pdf)
- [Autolykos PoW scheme specification]( https://docs.ergoplatform.com/ErgoPow.pdf)



# ZK Treasury

## Proposed Nautilus ZK Treasury

This basic concept is to create a visual programming toolkit to assist developers in learning and developing contracts in the EUTXO model. 

This toolkit will initially be built on top of Ergo Playground.  

The goal is to take advantage of the free composability offered by EUTXO. Create an open source library of visual, composable tools to onboard new developers. 

The “long term” goal is to create a headless central management system for developers, and a front-end UI focused central management system for basic users that are both interoperable with this visual programming toolkit. 

The name Nautilus is inspired by the Submarine in Jules Verne 20,000 Leagues Under the Sea. Nautilus is described by Verne as "a masterpiece containing masterpieces", which was built in secrecy, sourcing parts from unnamed sources and roams the seas beyond the reach of land-based governments.





---
title: NiPoPoWs
description: 
published: true
date: 2021-02-24T09:25:03.986Z
tags: 
editor: undefined
dateCreated: 2021-02-24T08:18:28.474Z
---

# NiPoPoWs
Several years have been spent researching and developing secure protocols that allow for efficient SPV clients. The two best-known and most reliable protocols are NiPoPoWs and FlyClient.

Ergo implements NiPoPoWs, or Non-interactive Proof-of-Proof-of-Work. This technology can be explored in full on [nipopows.com](https://nipopows.com/)

> Non-Interactive Proofs of Proof-of-Work (NIPoPoWs) are short stand-alone strings that a computer program can inspect to verify that an event happened on a proof-of-work-based blockchain without connecting to the blockchain network and without downloading all block headers. For example, these proofs can illustrate that a cryptocurrency payment was made.
>
> NIPoPoWs allow very efficient mobile wallets to be created. SPV wallets are already very lightweight compared to full nodes because they only require the download of block headers, not the whole blockchain. NIPoPoW wallets need to download only a small sample of block headers, around 250, when SPV clients need to download half a million block headers. The sample needed changes but doesn't grow much in size as the blockchain grows larger by the years, even after decades of data has been accumulated.

This enables Ergo to build a mobile SPV client that requires around just 100KB of block headers to be downloaded.

A super-efficient Ergo wallet with SPV security is in development, so stay tuned for more updates! 
[Building Ergo: SPV security](https://ergoplatform.org/en/blog/2020_05_1_spv_security/)

# Ergocast
 Dionysis Zindros, explains technical landscape of Non-Interactive Proofs of Proof-of-Work. Dionysis takes a diligent approach for the Ergo Cast with an elaborate rundown of what Non-Interactive Proofs of Proof-of-Work truly are. Furthermore, Dionysis evaluates the operation, implementation, as well as impact that his primitive delivers upon. Furthermore, we unveil a brand-new piece of research that -as of yet- has never been shared publicly: log-space mining.

[NiPoPoWs & Log-Space Mining – Ergo Cast Episode #5](https://ergocast.io/episode/nipopows-ergo-cast-episode-5/)

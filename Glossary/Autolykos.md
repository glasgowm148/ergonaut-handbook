---
title: Autolykos
description: 
published: true
date: 2022-09-13T08:40:06.545Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:34:47.337Z
---

# Autolykos


*Autolykos: The Ergo Platform PoW Puzzle* is a Proof of Work algorithm, but has several meaningful differences from Bitcoin's PoW. 

- Autolykos is memory-hard, reducing the disparity between specialized hardware (ASICs) and commodity GPUs, allowing ordinary people to participate in mining to secure the network and receive a reward.
- Autolykos difficulty adjustment uses the **linear least square method**, which smoothes over eight epoch's (each epoch is 1024 blocks x 2 minutes), as described in [this paper](https://eprint.iacr.org/2017/731.pdf). Autolykos makes difficulty adjustments slowly, but this helps prevent adversarial coin hopping. Autolykos has a 1.9% error rate compared to bitcoins 9.1% error rate (exponential 10% hash rate growth). 
- Autolykos v1 was originally pool resistant. However, it became apparent that it's impossible to prevent pools with smart contracts, so they (over 90% of miners) voted to disable Ergo's pool resistance so larger players could not take advantage of the loophole. 

More information available on [docs.ergoplatform.org](http://docs.ergoplatform.org/dev/protocol/autolykos/)

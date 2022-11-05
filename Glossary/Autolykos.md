---
title: Autolykos
description: 
published: true
date: 2022-11-05T11:59:39.657Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:34:47.337Z
---

# Autolykos


*Autolykos: The Ergo Platform PoW Puzzle* is a Proof of Work algorithm, but has several meaningful differences from Bitcoin's PoW. 

- Autolykos is memory-hard, reducing the disparity between specialized hardware (ASICs) and commodity GPUs, allowing ordinary people to participate in mining to secure the network and receive a reward.
- Autolykos originally adjusted difficulty using the **linear least square method**, which smoothed over eight epoch's (each epoch is 1024 blocks x 2 minutes), as described in [this paper](https://eprint.iacr.org/2017/731.pdf).     - Autolykos v2 now uses predictive linear least squares method which makes difficulty adjustments 87% faster than original Autolykos difficulty algorithm. 
- Autolykos v1 was originally pool resistant. However, it became apparent that it's impossible to prevent pools with smart contracts, so they (over 90% of miners) voted to disable Ergo's pool resistance so larger players could not take advantage of the loophole. 

More information available on [docs.ergoplatform.org](https://docs.ergoplatform.com/mining/autolykos/)

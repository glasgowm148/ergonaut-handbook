---
title: Autolykos
description: 
published: true
date: 2022-01-02T12:26:51.227Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:34:47.337Z
---

# Autolykos


Autolykos is a Proof of Work algorithm, but has several meaningful differences from Bitcoin's PoW. 

- It is memory-hard reducing the disparity between specialized hardware (ASICs) and commodity GPUs, allowing ordinary people to participate in mining to secure the network and receive a reward.
- Ergo uses the **linear least square method**, which smoothes over eight epoch's (each epoch is 1024 blocks x 2 minutes), as described in [this paper](https://eprint.iacr.org/2017/731.pdf). Autolykos will adjust slowly, but it also helps prevent **adversarial** hopping.

More information available on [docs.ergoplatform.org](http://docs.ergoplatform.org/dev/protocol/autolykos/)
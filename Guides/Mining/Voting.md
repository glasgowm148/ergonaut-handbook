---
title: Governance & Miner Voting
description: Many parameters can be changed on-the-fly via miners voting
published: true
date: 2022-09-15T07:47:46.925Z
tags: mining, vote, governance, mining vote
editor: markdown
dateCreated: 2022-09-10T05:40:16.859Z
---

# Governance 
Ergo Miners have the ability to adjust the block size which increases the amount of transactions per block. This increases potential rewards but also adds additional storage requirements. Maximum block size is just one of the 8 "everyday" changes possible on Ergo, as described below.

**Everday Changes `Id 1-8` require simple majority of votes to pass**:

**Id**|**Description**|**Default Value**|**Adjustment Step**|**Min Value**|**Max Value**|
|:-|:-|:-|:-|:-|:-|:-|:-|
|**1**|Storage fee factor (per byte per storage period)|1250000 |25000|0|2500000|
|**2**|Minimum monetary value of a box|360|10|0|10000| 
|**3**|Maximum block size|524288|-|16384|-|
|**4**|Maximum cumulative computational cost of a block|1000000|-|16384|-|
|**5**|Token access cost|100|-|-|-|
|**6**|Cost per one transaction input|2000|-|-|-|
|**7**|Cost per one data input|100|-|-|-|
|**8**|Cost per one transaction output|100|-|-|-|
   
______

In addition to the above "everyday" changes that can be changed via on-chain miner voting, most things on Ergo can be changed via soft-forking protocol (90% support required). Ergo miners have the ability to adjust the emission macroeconomics, meaning the long term economic security of the protocol is up to miners to decide. One notable example of this is [EIP-0027](https://github.com/ergoplatform/eips/blob/master/eip-0027.md). "Foundational" changes (implemented via soft-fork) **exclude critical changes such as changing the max supply.**

**Foundational Changes `Id 120`  require super majority (>90%) of votes to pass**:

**Id**|**Description**|**Default Value**|**Adjustment Step**|**Min Value**|**Max Value**|
|:-|:-|:-|:-|:-|:-|:-|:-|
|**120**|Soft-fork (increasing version of a block)| - |- | - |-|`

________
##### Original voting text (from yellow paper) has more details and some example votes to explore: https://github.com/ergoplatform/ergo/blob/master/papers/yellow/voting.tex


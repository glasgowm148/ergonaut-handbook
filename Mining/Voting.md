---
title: Governance & Miner voting
description: Many parameters can be changed on-the-fly via miners voting
published: false
date: 2022-09-15T05:51:07.581Z
tags: mining, vote, governance, mining vote
editor: markdown
dateCreated: 2022-09-10T05:40:16.859Z
---

# Governance 
Ergo Miners have the ability to adjust the block size which increases the amount of transactions per block. This increases potential rewards but also adds additional storage requirements. adjust the emission macroeconomics, meaning the long term economic security of the protocol is up to miners to decide.



    Id & Description & Default & Step & Min & Max \\

    \hline

    1 & Storage fee factor (per byte per storage period) & 1250000 & 25000 & 0 & 2500000 \\

    2 & Minimum monetary value of a box & 360 & 10 & 0 & 10000 \\

    3 & Maximum block size & 524288 & - & 16384 & - \\

    4 & Maximum cumulative computational cost of a block & 1000000 & - & 16384 & - \\

    5 & Token access cost & 100 & - & - & - \\

    6 & Cost per one transaction input & 2000 & - & - & - \\

    7 & Cost per one data input & 100 & - & - & - \\

    8 & Cost per one transaction output & 100 & - & - & - \\

   


In addition to the protocol parameters above that can be changed via on-chain miner voting, most things on Ergo can be changed via a soft-forking protocol (90% support required). This excludes critical changes such as changing the max supply.

 `120 & Soft-fork (increasing version of a block) & - & - & - & - \\`

---
title: Autolykos
description: 
published: true
date: 2021-03-27T11:31:20.673Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:34:47.337Z
---

# Autolykos


# v.2

Autolykos v.2 is following Autolykos v.1, but with certain modifications made:

-  non-outsourceability switched off. It turns out (based on more than 1 year of non-outsourceable PoW experience) that non-outsourceable PoW is not attractive to small miners.
-  now algorithm is trying to bind an efficient solving procedure with a single table of ~2 GB (initially), which is significantly reducing memory optimizations possibilities
- table size (memory requirements of a solving algorithm) grows with time
- The table depends solely on the block height, so there is no penalization for recalculating block candidate for the same height

Autolykos v.2 is briefly described at [Autolykos:  The Ergo Platform PoW Scheme](https://www.docdroid.net/mcoitvK/ergopow-pdf)

https://eprint.iacr.org/2020/044.pdf
---
title: Autolykos
description: 
published: true
date: 2021-03-27T11:34:59.265Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:34:47.337Z
---

# Autolykos


Security  of  Proof-of-Work  blockchains  relies  on  multiple  miners  trying to produce new blocks by participating in a *PoW puzzle lottery*,  and the network is secure if the majority of them are honest.  However, the reality becomes much more complicated than the original one-CPU-one-vote idea from the Bitcoin whitepaper\.

The first threat to decentralization came from mining pools – miners tend to unite in mining pools. Regardless of the PoW algorithm number of pools controlling more then 50% of computational power is usually quite small:  4 pools in Bitcoin, 2 in Ethereum, 3 in ZCash, etc.  This problem led to the notion of non-outsourceable puzzles. 

These are the puzzles constructed in such a way that if a mining pool outsources the puzzle toa miner, miner can recover pool’s private key and steal the reward witha non-negligible probability.  However the existing solutions either have too large solution size (kilobyte is already on the edge of acceptability fordistributed ledgers) or very specific and can not be modified or extendedin any way without breaking non-outsourceability. The second threat to cryptocurrencies decentralization is that ASIC-equipped miners are able to find PoW solutions orders of magnitude fasterand more efficiently than miners equipped with the commodity hardware.In order to reduce the disparity between the ASICs and regular hardware,memory-bound computations where proposed in. 

The most interesting practical examples are two asymmetric memory-hard PoW schemes which require significantly less memory to verify a solution than to find it. Despite  the  fact  that  ASICs  already  exist  for  both  of  them,  they remain the only asymmetric memory-hard PoW algorithms in use. 

Autolykos v.2 is briefly described at [Autolykos:  The Ergo Platform PoW Scheme]


# v.2

Autolykos v.2 is following Autolykos v.1, but with certain modifications made:

-  non-outsourceability switched off. It turns out (based on more than 1 year of non-outsourceable PoW experience) that non-outsourceable PoW is not attractive to small miners.
-  now algorithm is trying to bind an efficient solving procedure with a single table of ~2 GB (initially), which is significantly reducing memory optimizations possibilities
- table size (memory requirements of a solving algorithm) grows with time
- The table depends solely on the block height, so there is no penalization for recalculating block candidate for the same height

**Basic Ideas:**

- Like Autlykos-1, based on k-sum problem, so a miner needs to finds k (k=32) out of N (2^n = 2^26) elements, and hash of their sum must be less than target value (inverse of difficulty)
- k indexes are pseudorandom values derived from block candidate and nonce
- N elements are derived from block height and constants just, unlike Autolykos v.1, so miners can recalculate block candidates easily now (so only indexes are depending on them)
- Indexes calculation also involving the same table (which elements are last 31 bytes of H(i | | h | | M ), where i is in [0, N), h is block height, M is padding to slow down hash calculation (8kb of constant data).

So algorithm trying to make mining efficient for ones who store the table which size is 2^26 * 31 = 2,080,374,784 bytes initially (about 2GB). Thus algo now is friendly to all the GPUs basically.

Also, table size (N value) is growing with time as follows. Until block 614,400, N = 2^{26} = 67,108,864 elements (31 bytes each). From this block, and until block 4,198,400, every 51,200 blocks N is increased by 5 percent. Since block 4,198,400, value of N is fixed and equals to 2,143,944,600. Test vectors for N values are provided in the paper.

(https://www.docdroid.net/mcoitvK/ergopow-pdf)

https://eprint.iacr.org/2020/044.pdf
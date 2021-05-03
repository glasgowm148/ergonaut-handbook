---
title: Autolykos
description: 
published: true
date: 2021-05-03T10:47:12.642Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:34:47.337Z
---

# Autolykos


Security  of  Proof-of-Work  blockchains  relies  on  multiple  miners  trying to produce new blocks by participating in a *PoW puzzle lottery*,  and the network is secure if the majority of them are honest.  However, the reality becomes much more complicated than the original one-CPU-one-vote idea from the Bitcoin whitepaper\.

The first threat to decentralization came from mining pools – miners tend to unite in mining pools. Regardless of the PoW algorithm number of pools controlling more then 50% of computational power is usually quite small:  4 pools in Bitcoin, 2 in Ethereum, 3 in ZCash, etc.  This problem led to the notion of non-outsourceable puzzles. 

These are the puzzles constructed in such a way that if a mining pool outsources the puzzle toa miner, miner can recover pool’s private key and steal the reward witha non-negligible probability.  However the existing solutions either have too large solution size (kilobyte is already on the edge of acceptability fordistributed ledgers) or very specific and can not be modified or extendedin any way without breaking non-outsourceability. The second threat to cryptocurrencies decentralization is that ASIC-equipped miners are able to find PoW solutions orders of magnitude fasterand more efficiently than miners equipped with the commodity hardware. In order to reduce the disparity between the ASICs and regular hardware,memory-bound computations where proposed in. 

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


## 51% Attack

Mining pools offer a buffer against such network attacks as the hash rate is distributed across thousands of individual miners.

The memory hardened aspect of ergo also makes this vector of attack more expensive as there is no ASIC support to rent. With the collective rentable rigs at the moment this isnt a viable path to a 51% attack. In theory, someone could build a massive GPU farm to try to launch such an attack. If a bad actor can rent a warehouse of ASIC and mine on a small chain with 51% attacks are a viable option... if there is an offramp. 

Usually, this attack is done for profit and there is massive dumping that occurs on an exchange as it is occuring. Meaning the attacker is going to dump tokens on an exchange then "double-spend" them back into their wallet. The current exchange situation doesn't provide the liquidity for a viable offramp. The rentable ASIC support isn't an option. So is it possible, in theory, yes, practical or likely I dont think so at all.

Ethereum classic is perhaps a bad example, as it shares the same mining algorithm as Eth. One could buy more than 100% existing hashrate of eth classic on NiceHash. It's not the same case for Ergo. Ergo also believes in the 'Good Miner' principle, In the case of Bitcoin - it was a good thing 51% existed. 

Autolykos v1 originally had non-outsourcability built-in, however, it became apparent that with smart contracts it's basically impossible to prevent pools, so they turned it off so that not only larger players were able to take advantage of the loophole. Ergo is now focusing on memory hardness in an attempt to keep mining as fair as possible, which should help prevent ASICs mining at least. There are also some improvements for pooling, e.g. Stratum 2 protocol

“Bypassing Non-Outsourceable Proof-of-Work Schemes Using Collateralized Smart Contracts” https://ia.cr/2020/044 was presented by Alex Chepurnoy at WTSC workshop associated with Financial Cryptography and Data Security 2020 in Malaysia

It's also discussed here on 'Unblocked with Robert Kornacki' [(14:45)](https://www.youtube.com/watch?v=2sbTMrQwWOw&feature=youtu.be)
---
title: Use Cases
description: 
published: true
date: 2021-03-02T20:22:13.474Z
tags: 
editor: markdown
dateCreated: 2021-03-02T18:20:54.146Z
---

> *Ergo enables new models of financial interaction, underpinned by smart contracts built on flexible and powerful Sigma protocols but easily accessible to developers.*
{.is-info}


One of the most exciting things about blockchain is the possibility of making digital agreements without any trusted intermediaries. In the simplest use case, pioneered by Bitcoin, Alice can send a payment directly to Bob, wherever the two of them are located around the world, with no bank or any trusted third party needed. However, with the functionality of a modern blockchain like Ergo, it is possible to make far more complex and sophisticated financial agreements than simple payments. Take the following example.

# **Gold-backed tokens**
Alice uses ERGs to purchase gold-backed tokens from Bob. Bob stores the gold in a secure vault, and uses the blockchain to issue one token for every Troy ounce of gold he has. Alice can then use these tokens freely in different contracts, transferring and trading them under whatever conditions she specifies in the smart contract code. When Alice wants to sell the tokens for physical gold, she can conduct another transaction with Bob, receiving ERG in return, at market price.

The point of blockchain contracts is to eliminate the need for trust. While the purchase transaction is now trustless, in this instance Alice still needs to trust Bob about two things. Firstly, Bob may refuse to swap the gold tokens back to ERG at the correct price when Alice wants to sell. Secondly, Bob may default on his obligations – running away with the gold, or misusing the funds he receives and running a fractional reserve.

# **Extending the contracts**
To address these issues, we can create an Oracle, or decentralised price feed. This uses multiple sources of external data to record the price of gold to the blockchain at regular intervals. This price feed will be the reference point for the redemption contract that manages the sale of Alice’s gold with Bob (or any other participant). Thus the system automatically enforces the right price when a swap takes place.

The second situation requires a third-party insurer, Charlie, whose service is also hosted on the blockchain with a smart contract. When Alice purchases gold from Bob, she additionally buys an insurance contract from Charlie. The payment can be dependent on factors including the amount of insurance required, and Bob’s reputation – again, managed by a decentralized feedback mechanism. Now, if Bob defaults, Alice will automatically receive the value of her gold tokens, with Charlie effectively acting as a buyer of last resort.

# **Programmable contracts**
There are, of course, many other example use cases like this one. We can also extend this use case, adding further economic actors. For example, Charlie may sell shares in his insurance business to Dave and other participants, providing them with a proportion of revenues in return for ensuring he has the capital he needs to cover any liabilities from the outset.

However, even the most complex use case is simpler than general-purpose software that can be used to program any contract. After all, generalised logic must be both far-reaching and secure. Moreover, even a specialised contract is made up of many steps, each of which is fairly simple. Thus another requirement for a general-purpose platform is that it should simplify the process of writing contracts, making them as accessible (and safe) as possible. This can be achieved with the use of template agreements, with customisable parameters. The insurance contract above could be based on a module with flexible parameters, for example. This could be used and reused in many different circumstances.

# **Ergo’s approach**
This is essentially the approach that Ergo takes, providing superior support for real-world financial agreements. It does this through:

1. Support for multi-stage contracts (watch details for developers)
2. A simple high-level language, ErgoScript, enabling clear descriptions of contractual logic
3. Support for formal verification of contracts for improved security guarantees (Ergo Platform deployed its first formally verified p2p crowdfunding contract just three months after the network launched)
4. Easy Oracle creation
5. Native support for complex signature schemes


In short, creating financial contracts on the blockchain isn’t just about the functionality you provide. It’s about making that functionality safe and accessible, as well as powerful. Ergo achieves this and more.

# ‘hot potato’ monetary policy
> *As the next financial crisis takes hold, it’s clear that conventional monetary policy is at its limit. Smart contract platforms like Ergo enable more innovative, targeted implementations of economic stimulation that the conventional banking sector cannot achieve.*
{.is-info}

Conventional monetary policy is a hammer. It works as far as it goes, but if all you have is a hammer then every problem starts to look like a nail.

When the Global Financial Crisis hit over a decade ago, central banks did what they were used to doing. Cutting interest rates means it’s cheaper to borrow money, so there’s more cash in the system that can be spent and will circulate in the economy – paying for goods and services, funding employment and allowing life to continue something like as normal.

That, at any rate, is the theory. It’s what central banks do in recessions to stimulate economic activity. When times are better, they raise interest rates to make it more expensive to borrow money and prevent the economy from overheating (including asset bubbles).

## **The outer limits**

This is a blunt tool, but it works, up to a point. In the 2008 crisis, the problem was more severe – so severe, in fact, that interest rates were slashed to zero. Banks were still afraid to lend because they didn’t know the quality of the collateral they were offered in return, those notorious mortgage-backed securities.

So the central banks undertook a programme of Quantitative Easing (QE). This entailed creating huge amounts of cash that didn’t exist before, then purchasing various assets from the banks. The idea was that the central bank would take on the risk and the assets, and commercial banks would then use this gift of liquidity to lend to small businesses and individuals, allowing them to continue operating as before.

It didn’t work. Little of that newly-created money went to small businesses. Instead, banks used it to shore up their own balance sheets and make their own finances safer, investing only in low-risk assets rather than risky SMEs. Ultimately that cash filtered through to assets like the stock market and property, making the wealthy even more wealthy while the poorer were priced out of the market.

## **Helicopter money**

Today, as we experience the greatest financial challenge of our lifetimes – greater than even the Global Financial Crisis – central banks are considering even more unorthodox approaches. One of these is ‘helicopter money’. This involves cash being simply airdropped directly to citizens, either in the form of tax breaks or as money straight into their bank accounts. America has discussed giving $1,200 to every adult. Other nations are exploring the same idea.

But there’s a problem with this, too.

Just like the banks, ordinary citizens are worried about their finances. So instead of going out and spending (where ‘going out’ is even possible), they pay down their debt. That newly-printed money goes nowhere.

That’s really as far as central banks can go. But a platform like Ergo can offer different types of money, with different conditions attached via smart contracts, incentivising different behaviour in different circumstances. And that enables a whole different range of monetary policy tools.

## **‘Hot potato’ money**

In normal times, banks seek to maintain an inflation rate of around 2%. This means money is worth less over time. So instead of saving it all, and seeing the value of their savings fall, citizens have the incentive to spend it and circulate it within the economy.

Too much inflation, of course, is a bad thing. Get money printing wrong and you have hyperinflation like Venezuela or Zimbabwe, and your economy collapses.

But what if we kept inflation low, but created a limited amount of a special class of money that had to be used quickly if it was to retain its value at all? We’ll call this ‘hot potato’ money, because it has to be passed on fast.

Using a blockchain and smart contracts, this would be a simple matter of creating a new token that could be freely transferred and traded, just like any other token. And it could be backed by reserves (held with the central bank, commercial banks or any other entity). But the difference would be that it has to be spent within a month of receiving it, or those tokens are locked, their value is lost to the holder and the funds that back them are freed up to return to the reserve holder.

So this would be regular money that people had to spend: use it or lose it. If they hoard it, it becomes useless. And we can ensure that it is not used to pay down debt by including conditions that ensure it cannot be used by the banking sector. Of course, Ergo’s Sigma protocols can be used to figure out what has been spent, where, without knowing individual spending habits – enabling even more targeted stimulus.

This idea likely has far-reaching implications – and possibly unintended consequences. What would the result be, for example, of creating different ‘classes’ of money that were only semi-interchangeable? Would this introduce unwelcome, even dangerous friction?

This and other questions would need to be explored further. What’s clear is that central banks are already experimenting with unconventional monetary policy and are fast reaching the end of the road. We can continue that experiment with better, more powerful and targeted tools.


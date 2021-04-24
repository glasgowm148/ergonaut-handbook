---
title: Sigma-FAQ
description: 
published: true
date: 2021-04-24T12:03:27.187Z
tags: 
editor: markdown
dateCreated: 2021-03-04T19:07:06.877Z
---


# FAQ
## Sigmausd.io Purchase

1. Visit [SigmaUSD.io](https://sigmausd.io/#/)
2. Connect your wallet. This will be used to store your Sigma, any transaction refunds or withdrawals. 
3. Go to the SigmaRSV/SigmaUSD page. RSV is too long Erg, USD for stability or too short Erg.
4. Enter the amount desired, use the calculator to get a grasp on the ratios.
5. You'll be prompted with an address and an amount to send
6. The transaction should appear within your transaction history on the homepage within a few minutes. Green means the operation passed, red means it failed. 
7. Your funds will automatically be sent 

>The bootstrap period where the reserve ratio can go above 800% lasts until block 450k (about the end of March) - [You can view the block height here](https://explorer.ergoplatform.com/en/). You'll be able to keep them in there or redeem them and get your Ergs back. You just won't be able to mint more sigRSV once the bootstrap period finishes if the reserve ratio is > 800%
{.is-info}



## If Erg goes 10x, can I get 10x more Erg?

If people are minting and redeeming stablecoins a lot in future, the 1% fee can add up quickly. Your return ratio depends on many factors such as when you entered, when you exit, the oracle price fluctuations, the initial reserves, the total amount of SigmaUSD in reverse. 


You have to go through the equations and run them with a specific scenario to predict the exact return. 

> SigRSV is a [**reserve**](https://explorer.ergoplatform.com/en/addresses/2zYVHmdQDGtyyZfeqFPdMFqWzMdK299yCj5uDJjiSxRgpHyjiV3mVfZCimFbEVkNkCuypT1khjhupnEb6af3ztdatgag24UzLjW7heidiBF4MqK42TBZC1mLNcm851kvjaEwMsm8bnT2ZwJ6g18ZdDtdKTqEq7KBtp9gkvXiScoNNrA55JhC5o1ZdKRfjRqKMsfWBqmUqTNZfLXy62ddoP8oGT6HafqzKp9YLdSr172KYsnJoK3MhRciMG3McYHfkCFzT3fgNiaTosEtDKUSxaDEmY3r6eTF5H1QmYdkDfEe9AGxzjPgcwR19CfTkuGt8Xg3iUnLRciZ6hVBJc642qDR1EBjY8g7sAtestKYxRLKvUrjV9o3rbFccpgREynwf63mHUZ2jFnuuP2YfeJZdhPf6eK7dnLQ6HDkq5JBd76G7ErB17V1yCr7J6DrC6m47B8aY1XU5fFFQ6Hy6fJm7jzb5DHdn3U4V3TdUM5WwMe6hAmTBz3kFtJBKAiqTw5g53doV7CuUWqC9fTKhGo3BYfXtjFCxeJLwxsXx91s5MWT4tST4XBFnoJP6SZKkfuW7ZvtRbcgpVsz37X6o7YxitwNzaDNmkR9GVLU1XK4cQZjfBijQrTXTTApXnq6wPzzvHTgKyxVuQdDcniEDcgQwttTX4mqooCqxshjy79XL3sFCSTxh4Pjm9UjCgq9daTn83Ro2LnHHifaMjXpFGAbySvqwNvxwBHJnsTXKh2fRggxLDLVobBUfq7DxssPfSaeF4exmdU3mhtuhVhFxAaUVY3LBigWcm4642GtzECVmFRLy1y96m7utcqBiMoyNDy8K3hrM6uzpnA5VYuC6s3jqYp6wZ95QCcRyc3roZL6qTrRXiJupiwYXL3FA1THXPAXLm3PgM7VosJth3bj). If SigUSD holders withdraw at a lower price than they entered, the reserve makes up the difference.
{.is-warning}

Here is an advanced [introduction to ERGO's SigmaUSD stablecoin risk and reward mechanism.](https://veriumfellow.medium.com/introduction-to-ergos-sigmausd-stablecoin-risk-and-reward-mechanism-18690b52d672)

## Why would anyone buy SigUSD?

**SigmaUSD is a call option on the dollar amount held in reserves.** So if the price of ERG drops, the same amount of $ buys more ERG


This offers decentralised liquidity for miners and large holders who can choose to mint SigUSD to ensure they can always redeem the dollar value - while keeping the option to quickly buy back into Erg on an unexpected dip. 

SigmaUSD also serves a second purpose when there is a Defi ecosystem; 

If price appreciation runs past the opening position of SigmaUSD, the short position offers no gain in ERG but does become a useful stablecoin.

An example, if ERG doubled, there is no incentive for SigmaUSD holders to close a short at a loss of ERG. The incentive changes to build an ecosystem that gives further utility or return to that stable locked value. This creates a market incentive to build a further utility for SigmaUSD. 

Ergonauts can support the network by 'cashing out' into SigmaUSD. It's important to remember that this is still a bull run; it is wise to set cash-out points.

An example; Someone who invested $1000 may set a 'cash-out' point at $10,000 where they withdraw their initial investment. This prevents complete loss in the event of a market crash. Using SigmaUSD for this purchase means this can be done decentralised, without dealing with an exchange - and also gives you the bonus of easily redeeming bonus ergs if the market dips and you want to take profits. It's essentially a very low-risk short position as you can never be liquidated and will never actually loose dollar value. 


# My transaction failed
There is currently significant demand. With Ergo being in the UTXO model and all of the dApp design patterns being quite young, we have limitations for the throughput. We have many high-level design ideas to address this for the future, with asynchronous EUTXO protocols, but this is still being deeply researched. 

We decided that it was better for the community to have something in the near term rather than waiting another year for the research to solidify into an implementation.


# My profits are lower than expected

SigRSV is a **long** position, shorters were able to use their volume to profit off the dips during the initial launch. Their ability to do so has been reduced now so transactions will be building up at a faster rate. 

[SigmaUSD DAO bank is a complex beast - ergoforums.org](https://www.ergoforum.org/t/sigmausd-dao-bank-is-a-complex-beast/767)

# Why are the fees so high?

> The fee to close a MakerDAO CDP and return your dai is currently 8.5%
{.is-danger}

Fees are set at 2.25%. 2% goes directly back to the reserves and 0.25% for the frontend implementation implementors. 

If you mint sigmaRSV, you get that 1% back anyways since your reserve coins match the reserve. The more SigRSV you buy, the lower that fee is for you since you own a larger portion of the reserves.


SigmaUSD still lacks a mature DeFi ecosystem, with 1% of each transaction going to the reserves as the price appreciation, there is potential for a large return. 



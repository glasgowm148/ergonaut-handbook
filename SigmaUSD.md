---
title: SigmaUSD
description: 
published: true
date: 2021-02-27T19:20:51.376Z
tags: 
editor: undefined
dateCreated: 2021-02-24T08:02:25.004Z
---

> Introducing [SigmaUSD.io](https://sigmausd.io/#/) the first UTxO-based stable coin - an instantiation of the [AgeUSD protocol](https://github.com/Emurgo/age-usd). The foundation on which a new era of digital finance will be built. 
{.is-success}

> There is currently significant demand . With Ergo being in the UTXO model and all of the dApp design patterns being quite young, we have limitations for the throughput. We have a lot of high level design ideas to address this for the future, with asynchronous EUTXO protocols, but this is something that is still being deeply researched. 
>
>As such we decided that it was better for the community to have something in the near term rather than waiting another year for the research to solidify into an implementation. - Robert k
{.is-warning}


IOHK, Ergo, and Emurgo designed the economic model of SigmaUSD. Its economic model maintains the conservative settings for collateral reserves and avoids the need for liquidations. Along with that, it supports a fully decentralised stablecoin emission setup. Thus, SigmaUSD will offer the world a stable, simple, and decentralised stablecoin.

## ELI5
Everyone struggles to get their head around this concept — so here's an ELI5 version without the checks-and-balances to start you off. 

**Assuming Erg is $1;**

- You take 100 ERG worth $1 each and mint them into either StableCoins or ReserveCoins
- If you mint SigmaRSV, and the price goes up 10% — you get back 110 ERG when you cash out.
- If you mint into the SigmaUSD, and the price goes up 10% — you still get $100 out, but because its went up 10%, you get 90ERG

> This provides individuals with the ability to choose to either go **long** on Erg by minting **SigmaRSV** or to choose **stability** by minting **SigmaUSD.**
{.is-info}



## ELI5 - Sigma Purchase

1. Visit [SigmaUSD.io](https://sigmausd.io/#/)
2. Connect your wallet. This will be used to store your Sigma, any transaction refunds or withdrawals. 
3. Go to the SigmaRSV/SigmaUSD page. RSV is to long erg, USD for stability or to short erg.
4. Enter the amount desired, use the calculator to get a grasp on the ratios.
5. You'll be prompted with an address and a amount to send
6. The transaction should appear within your transaction history on the homepage within a few minutes. Green means the operation passed, red means it failed. 
7. Your funds will automatically be sent 

> There are some last minute growing pains being ironed out, and lots of people trying to get their hands on SigmaRSV. If your transaction failed, try again in a little bit. 
{.is-warning}


>The bootstrap period where the reserve ratio can go above 800% lasts until block 450k (about the end of March) 
{.is-info}

You'll be able to keep them in there, or redeem them and get your Ergs back. You just won't be able to mint more sigRSV once the bootstrap period finishes if the reserve ratio is > 800%

- [You can view the current reserve here](https://explorer.ergoplatform.com/en/addresses/2zYVHmdQDGtyyZfeqFPdMFqWzMdK299yCj5uDJjiSxRgpHyjiV3mVfZCimFbEVkNkCuypT1khjhupnEb6af3ztdatgag24UzLjW7heidiBF4MqK42TBZC1mLNcm851kvjaEwMsm8bnT2ZwJ6g18ZdDtdKTqEq7KBtp9gkvXiScoNNrA55JhC5o1ZdKRfjRqKMsfWBqmUqTNZfLXy62ddoP8oGT6HafqzKp9YLdSr172KYsnJoK3MhRciMG3McYHfkCFzT3fgNiaTosEtDKUSxaDEmY3r6eTF5H1QmYdkDfEe9AGxzjPgcwR19CfTkuGt8Xg3iUnLRciZ6hVBJc642qDR1EBjY8g7sAtestKYxRLKvUrjV9o3rbFccpgREynwf63mHUZ2jFnuuP2YfeJZdhPf6eK7dnLQ6HDkq5JBd76G7ErB17V1yCr7J6DrC6m47B8aY1XU5fFFQ6Hy6fJm7jzb5DHdn3U4V3TdUM5WwMe6hAmTBz3kFtJBKAiqTw5g53doV7CuUWqC9fTKhGo3BYfXtjFCxeJLwxsXx91s5MWT4tST4XBFnoJP6SZKkfuW7ZvtRbcgpVsz37X6o7YxitwNzaDNmkR9GVLU1XK4cQZjfBijQrTXTTApXnq6wPzzvHTgKyxVuQdDcniEDcgQwttTX4mqooCqxshjy79XL3sFCSTxh4Pjm9UjCgq9daTn83Ro2LnHHifaMjXpFGAbySvqwNvxwBHJnsTXKh2fRggxLDLVobBUfq7DxssPfSaeF4exmdU3mhtuhVhFxAaUVY3LBigWcm4642GtzECVmFRLy1y96m7utcqBiMoyNDy8K3hrM6uzpnA5VYuC6s3jqYp6wZ95QCcRyc3roZL6qTrRXiJupiwYXL3FA1THXPAXLm3PgM7VosJth3bj)
- 
- [You can view the blockheight here](https://explorer.ergoplatform.com/en/)

### FAQ : If Erg goes 10x, can I get 10x more erg?

If people are minting and redeeming stablecoins a lot in future, the 1% fee can add up quickly. Your return ratio depends on a multitued of factors such as when you entered, when you exit, the oracle price fluctuations, the initial reserves, the total amount of SigmaUSD in the reverse. 


If you assume a static amount of ergs in the protocol, then the max would be however many Ergs are provided by the stablecoin owners and you hold all the reserve coins, and the erg price goes to infinity. There is no theoretical max technically

You have to go through the equations and run them with a specific scenario to predict the exact return. 

[Ergo Summit 2021 - The IOHK Perspective - Designing the AgeUSD StableCoin](https://youtu.be/zG-rxMCDIa0?t=9247)

### FAQ : Why would anyone buy SigUSD?
> SigmaUSD is a call option on the dollar amount held in reserves. So if the price of ERG drops, the same amount of $ buys more ERG
{.is-info}


Even though since launch, the price rose significantly - there were several large SigUSD buys shorting Erg. This offers decentralised liquidity for miners and large holders who can choose to mint SigUSD in order to ensure they can always redeem the dollar value - while keeping the option to quickly buy back into Erg on an unexpected dip. 

SigmaUSD also serves a second purpose when there is a Defi ecosystem; 

If price appreciation runs past the opening position of SigmaUSD the short position offers no gain in ERG... but does become a useful stablecoin.

An example; if ERG doubled there is no incentive for SigmaUSD holders to close a short at a loss of ERG. The incentive changes to build an ecosystem that gives further utility or return to that stable locked value. This creates market incentive to build further utility for SigmaUSD. 



### Fees

Fees are set at 1.25%. 1% goes directly back to the reserves and 0.25% for the frontend implementation implementors. 

If you mint sigmaRSV you get that 1% back anyways since your reservecoins match the reserve. The more SigRSV you buy the lower that fee is for you since you own a larger portion of the reserves.

> The fee to close a MakerDAO CDP and return your dai is currently 8.5%
{.is-danger}

SigmaUSD still lacks a mature DeFi ecosystem, 1% of each transaction going to the reserves as the price appreciate, there is potential for a large return. 

## Overview
**Reserve Providers** submit Ergs to the dApp's reserves and by doing so mint ReserveCoins (**SigmaRSV**). Each SigmaRSV represent a portion of the underlying Erg reserves held in the dApp.

**SigmaUSD** Users also submit Ergs to the dApp reserves; however, in their case, they mint SigmaUSD instead. This is only allowed by the protocol if there are sufficient reserves within the dApp (reserves are above the minimum reserve ratio). At any given moment, a SigmaUSD user can redeem their SigmaUSD in exchange for an amount of Ergs from the reserves equal to the current exchange rate as sourced by the Erg-USD oracle pool.

Reserve Providers can only redeem their ReserveCoins for Ergs if the price of Ergs goes up (or a substantial amount of protocol fees are collected) and thus cover the value of all existing minted SigmaUSD plus an extra margin. By redeeming their ReserveCoins, they profit as they receive more underlying reserve cryptocurrency than when they minted their ReserveCoins (the increased amount coming from users who minted SigmaUSD).

> Reserve Providers allow SigmaUSD users to enjoy the stability of value. On their end, the Reserve Providers absorb the potential upside (if the value of the reserves goes up via the price of Ergs increasing compared to USD) and absorb the potential downside (if the underlying cryptocurrency in reserve goes down in price).
{.is-info}


## Advantages over MakerDAO
> **No liquidations!**
{.is-success}

Unlike Ethereum-based crypto-backed stablecoins, such as DAI, Emurgo introduces a Staticoin protocol-inspired design that does not rely on CDPs (Collateralized Debt Positions). The reason for this is the vulnerability of CDP-based protocols in terms of high volatility and blockchain congestion. As Emurgo states, "Black Thursday," when MakerDAO CDPs were triggered for liquidation due to volatility and then sold for $0 due to blockchain congestion that prevented others from bidding, demonstrated that a new design is needed. For SigmaUSD, this scenario is not possible.

As the community is going straight to the SigmaUSD-based stablecoin launch, we recommend again this impressive presentation by Bruno Woltzenlogel Paleo, "An IOHK Perspective: Designing The SigmaUSD Stablecoin Protocol — An Economic Analysis" from the ErgoSummit.




## Mining Incentives
> SigmaUSD offers a unique way for miners to create the base infrastructure for a robust DEFI system.
{.is-info}


Miners that maintain the network are the lifeblood of a robust POW system. A decentralised system will have a variety of actors that allow the system to grow. It is essential to consider the proper incentives to serve the needs of the community. Ergo is built on solid technological foundations; the decentralised financial market is made with historical foundations in mind.

Traditionally central banks held gold as reserves that backed currency. Currency was used as a stable medium of exchange throughout economies. When stable or backed by assets, this system of banking allowed commerce and growth.

We have moved away from a system in which currency is backed by anything. The global reserve currency is run on a banking system that has 0% reserve requirements. 

Governments around the world are in the process of continually feeding liquidity into the global economy. Central banks globally are creating money and debt at unprecedented rates. This debt will burden countless future generations, or debts will reach a default and restructuring point.

Digital Assets are a market alternative to the inflationary pressure of fiat currency. The "law" enshrined in the code creates scarcity at a predictable emission schedule. The resource in Ergo is ERG. Miners consume electricity and create this secure electronic asset.

In the global economy, gold is produced by miners and is sold to a variety of actors. Some gold miners may sell ore/refined product to open markets, create OTC contracts, or sell to the central bank to hold in reserve.

Ergo already has pathways to the open market via exchanges. OTC, dark pools and a DEX are in development for private P2P sales. SigmaUSD represents a 3rd option that allows miners access to liquidity, the ability to interact with a central contract or bank while circumventing the open market.

The economics of mining crypto is similar to the economics of trading. Some miners build long positions. They are project-oriented. They to find a project they believe in and provide critical network infrastructure, maintenance, and development.

Other miners act as freelancers; they provide critical services to profitable projects. They often do not build reserves and are continually liquidating in the open market to cover their production cost.

### Key Points

- SigmaRSV can offer project-oriented miners a way to maximise their positions by accumulating fees. This class of miners can naturally benefit from SigmaRSV.
- SigmaUSD can offer freelance miners liquidity to cover their expenses in a decentralised manner, free of exchanges. This class of miners can naturally benefit from SigmaUSD.
- SigmaUSD offers a somewhat hidden incentive for miners to create greater price stability in the asset they are assisting in creating and maintaining. Over time this builds to the robustness and resiliency of the network.
- PoW benefits from price stability. The core infrastructure providers (miners) operate on a Return on Energy Invested model. The base cost of this mode is Equipment and Energy.
- Price stability assist miners in predicting future costs/revenues. SigmaUSD can serve as a price stabilisation mechanism as miners interact with the contract based on their incentive. Long vs Liquidity.
- Interacting with this protocol rather than interacting with the open market is beneficial to all parties.
- The premise of ERGO has always been a PoW system that can operate as a Digital Reserve of Programmable Gold.

### ERG Reserve Threshold
- SigmaUSD is operated on larger margin requirements than traditional crypto-backed stablecoins. 
ERG will back-SigmaUSD in a floating reserve between 4x1 to 8x1.
- The minimum threshold (4x1) protects SigmaUSD holders; tokens are 

#### ALWAYS backed by sufficient ERG for market volatility.
- The maximum threshold (8x1) protects SigmaRSV holders from experiencing unnecessary dilution of their P/B position. This limits inflationary pressures on SigmaRSV holders.
- The SigmaUSD has locking mechanisms to keep the Reserves within this range. It is possible that users can temporarily find themselves unable to interact with the contract. This is the alternative to forced liquidations.
- The Federal Reserve Board reduced reserve requirement ratios to zero percent effective March 26, 2020. This action eliminated reserve requirements for all depository institutions.
- The global reserve currency is backed by 0% reserve ratios.
A MINIMUM 400% reserve ratio backs-SigmaUSD. 
# SigmaRSV (Reservecoin) Simplified
- SigmaRSV is a call option on a % of the ERG held in the reserve portion of the SigmaUSD contract
- Fees are continually added to the ERG held in reserve as users interact with the contract. This mechanism ensures liquidity and offers a mechanism of return beyond trading.  SigmaRSV represents a price/book (P/B Ratio) on the ERG held in reserve.

> It is important to understand three mechanisms that influence the outcome of each user of SigmaRSV 
{.is-info}

1. Fees accumulate as users interact with the contract. Nothing is Free. 
2. The amount of ERG held in reserve floats (up/down) as users interact with the contract.
3. The price ERG/USD floats (up/down) as users trade ERG.


### Overview

- Imagine the Reserve amount is 100 ERG.
- Alice holds SigmaRSV that represents 10% of the (P/B Ratio) contained in the reserves.
- Alice's SigmaRSV position is a call option on 10 ERG (minus the exchange fee)
- Let's imagine the price of ERG is 2$.
- Alice's SigmaRSV represents 20$ in ERG (minus the exchange fee)
#### THE BALANCE IN RESERVE CAN GO UP
- Imagine, based on use, the reserve now holds 114 ERG.
- Alice has SigmaRSV that represents 10% of the (P/B Ratio) contained in the reserves.
- Alice's SigmaRSV represents a call option on 11.4 ERG's.
- Let's imagine the price of ERG is still 2$.
- Alice has 22.80$ in ERG (minus the exchange fee)
#### THE BALANCE IN RESERVE CAN GO DOWN
- Imagine, based on use, the reserve now holds 90 ERG.
- Alice has SigmaRSV that represents 10% of the (P/B Ratio) contained in the reserves.
- Alice's SigmaRSV represents a call option on 9 ERG's.
- Let's imagine the price of ERG is still 2$.
- Alice has 18.00$ in ERG (minus the exchange fee)
#### THE VALUE, ERG/USD, CAN GO UP
- Imagine, based on use, the reserve now holds 114 ERG.
- Alice has SigmaRSV that represents 10% of the (P/B Ratio) contained in the reserves.
- Alice's SigmaRSV represents a call option on 11.4 ERG's.
- Let's imagine the price of ERG is still NOW 3$.
- Alice has a call option 34.20$ in ERG (minus the exchange fee)
#### THE VALUE, ERG/USD, CAN GO DOWN
- Imagine, based on use, the reserve now holds 114 ERG.
- Alice has SigmaRSV that represents 10% of the (P/B Ratio) contained in the reserves.
- Alice's SigmaRSV represents a call option on 11.4 ERG's.
- Let's imagine the price of ERG is still NOW 1$.
- Alice has a call option 11.40$ in ERG (minus the exchange fee)
#  SigmaUSD (Stablecoin) Simplified
> SigmaUSD represents a call option on the dollar value of ERG held in reserve. 
{.is-success}

SigmaUSD uses Ergo's oracle pools infrastructure to calculate and adjust the current ERG/USD exchange rate. 

Reserve always backs sigma USD. The price ERG/USD floats (up/down) as users trade ERG.


#### BASIC OVERVIEW
- Bobs has 20 SigmaUSD that represents 20 USD value in ERG.
- These ERG's are held in Reserve.
- This 20$ of value is backed by reserves of at least
- (4x1)(80$ of ERG)(40 ERG @ $2)
- Bob at 2$ Bob can Redeem his 20 SigmaUSD for 10 ERG (minus the exchange fee)
#### ERG/USD VALUE DROPS
- Let us imagine the price of ERG drops from $2 to $1.
- Bobs 20$ of value is backed by at least
- (4x1)(80$ of ERG)(80 ERG @ $1)
- Bob can call 20 ERG (minus the exchange fee)
#### ERG/USD VALUE INCREASES
- Let us imagine the price of ERG increases from $2 to $4.
- Bobs $20 of value is backed by at least
- (4x1)(80$ of ERG)(20 ERG @ $4)
- Bob can call 5 ERG (minus the exchange fee)


# Infographics

![screenshot_2021-02-25_at_19.14.01.png](/screenshot_2021-02-25_at_19.14.01.png)
![unknown.png](/unknown.png)


# Cardano on StableCoins

**Cardano's Stablecoin Will be 'Better Than MakerDAO,' Says Hoskinson**
> "For example, we've partnered with Emrugo, and we're right now working on the logistics of a stablecoin with them that we're going to be building first on Ergo to verify everything works correctly, and then we'll pull it over into Cardano and this is going to be an algorithmic stablecoin," said Hoskinson, adding, "We think it'll be significantly better than MakerDAO."

**'Will SigmaUSD launch with gougen?**
>'  I'm going to see if we can do a SigmaUSD port after we do native-assets; we already have a Plutus implementation. We're discussing a lot of legal and regularatory stuff. It's a high priority of mine because it's interconnected for what we'd like to do for the next generation of Cardano, and it's very important to pull those things together.

Charles answering '*are there use cases where PoW is better*'.

>Until we deploy Orboros Genesis, PoW is significantly better and unique vs PoS in that you don't need a checkpoint, which is a huge advantage...and if you desire to gain a lot of computational abilities, especially with async resistance, PoW is better as you're building a supercomputer
>We are definitely going to do a stablecoin. It's just when you say stablecoin; there are many different types of stablecoins. You have things like asset-backed stablecoins where Tether (USDT) is an example of that, where someone buys USD, and they store in a bank account and then for every USD you mint a tether. You have commodity-backed stablecoins like goldcoins or these things... You have metastable coins where you take a basket of stablecoins, and you create a synthetic asset that's backed by that basket, and then you have algorithmic stablecoins like the Maker DAOs, where some mechanic keeps the coins stable, and then you have central bank issue digital currencies which is a sexy hot topic, like the Marshall Islands for example. There's a whole spectrum there, and actually, we have teams who look at each of these. In Africa, in particular, many governments have come to us and said, hey, we want to do commodity-backed stable coins.
>
> We're excited about that, and when we talk about sovereign counter partners, there I think the best thing to do is couple stable coins with universal basic income (UBI). Basically, during the operation of the stablecoin, there are transaction fees, and you let those fees accumulate in a sovereign wealth account and then what you do is you periodically give dividends to all the people of the country for that. This is super attractive when you have a smaller jurisdiction, let's say a Mauritius or something like that, and they have a lot of problems, and it allows them to basically get a lot of direct foreign investment and then they can do a direct distribution to their people.
We are exploring those, and there's been a lot of excitement on these governments' monetary policy side. The big challenge is also the regulatory layer on top of stablecoins. There needs to be the ability to freeze them, reverse transactions in the compliance layer. Cardano has a unique advantage here in that we have a product called Prism, and it's our identity management stack. It's blockchain agnostic, but it's tightly integrated with Cardano. It's a layer two identity stack based on DIDs, and this is going to enable people to have things like authenticated addresses where you could associate an address or an asset with a DID. DID is a decentralised identifier; then you can do KYC and AML on that DID, and then suddenly you can create a transitive graph of ownership and verify that all the people touching it has the right to do that. Who signs that DID is completely neutral. You could have a government sign it; regulatory bodies sign it; you can have a private entity like Pwc sign it or something like that.

https://thedailychain.com/hoskinson-cardano-working-on-stablecoin-to-rival-makerdao-developing-defi-products/


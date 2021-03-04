---
title: SigmaUSD Overview
description: 
published: true
date: 2021-03-04T19:11:18.814Z
tags: 
editor: markdown
dateCreated: 2021-03-04T19:09:20.239Z
---

# Overview 
IOHK, Ergo, and Emurgo designed the economic model of SigmaUSD. Its economic model maintains the conservative settings for collateral reserves and avoids the need for liquidations. Along with that, it supports a fully decentralised stablecoin emission setup. Thus, SigmaUSD will offer the world a stable, simple, and decentralised stablecoin.

**Reserve Providers** submit Ergs to the dApp's reserves and by doing so mint ReserveCoins (**SigmaRSV**). Each SigmaRSV represent a portion of the underlying Erg reserves held.

**SigmaUSD** Users also submit Ergs to the dApp reserves; however, in their case, they mint SigmaUSD instead. This is only allowed by the protocol if there are sufficient reserves within the dApp (reserves are above the minimum reserve ratio). At any given moment, a SigmaUSD user can redeem their SigmaUSD in exchange for an amount of Ergs from the reserves equal to the current exchange rate as sourced by the Erg-USD [oracle pool](https://explorer.ergoplatform.com/en/oracle-pool-state/ergusd). 

Reserve Providers can only redeem their ReserveCoins for Ergs if the price of Ergs goes up (or a substantial amount of protocol fees are collected) and thus cover the value of all existing minted SigmaUSD plus an extra margin. By redeeming their ReserveCoins, they profit as they receive more underlying reserve cryptocurrency than when they minted their ReserveCoins (the increased amount coming from users who minted SigmaUSD).

> Reserve Providers allow SigmaUSD users to enjoy the stability of value. On their end, the Reserve Providers absorb the potential upside (if the value of the reserves goes up via the price of Ergs increasing compared to USD) and absorb the potential downside (if the underlying cryptocurrency in reserve goes down in price).
{.is-info}



### ERG Reserve Threshold
- SigmaUSD is operated on larger margin requirements than traditional crypto-backed stablecoins. ERG will back-SigmaUSD in a floating reserve between 4x1 to 8x1.
- The minimum threshold (4x1) protects SigmaUSD holders; **tokens are ALWAYS backed by sufficient ERG for market volatility.**
- The maximum threshold (8x1) protects SigmaRSV holders from experiencing unnecessary dilution of their P/B position. This limits inflationary pressures on SigmaRSV holders.
- The SigmaUSD has locking mechanisms to keep the Reserves within this range. It is possible that users can temporarily find themselves unable to interact with the contract. This is the alternative to forced liquidations.
- The Federal Reserve Board reduced reserve requirement ratios to zero percent effective March 26, 2020. This action eliminated reserve requirements for all depository institutions.
- The global reserve currency is backed by 0% reserve ratios.
- A minimum 400% reserve ratio backs-SigmaUSD. 

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

**THE BALANCE IN RESERVE CAN GO UP**
- Imagine, based on use, the reserve now holds 114 ERG.
- Alice has SigmaRSV that represents 10% of the (P/B Ratio) contained in the reserves.
- Alice's SigmaRSV represents a call option on 11.4 ERG's.
- Let's imagine the price of ERG is still 2$.
- Alice has 22.80$ in ERG (minus the exchange fee)

**THE BALANCE IN RESERVE CAN GO DOWN**
- Imagine, based on use, the reserve now holds 90 ERG.
- Alice has SigmaRSV that represents 10% of the (P/B Ratio) contained in the reserves.
- Alice's SigmaRSV represents a call option on 9 ERG's.
- Let's imagine the price of ERG is still 2$.
- Alice has 18.00$ in ERG (minus the exchange fee)

**THE VALUE, ERG/USD, CAN GO UP**
- Imagine, based on use, the reserve now holds 114 ERG.
- Alice has SigmaRSV that represents 10% of the (P/B Ratio) contained in the reserves.
- Alice's SigmaRSV represents a call option on 11.4 ERG's.
- Let's imagine the price of ERG is still NOW 3$.
- Alice has a call option 34.20$ in ERG (minus the exchange fee)

**THE VALUE, ERG/USD, CAN GO DOWN**
- Imagine, based on use, the reserve now holds 114 ERG.
- Alice has SigmaRSV that represents 10% of the (P/B Ratio) contained in the reserves.
- Alice's SigmaRSV represents a call option on 11.4 ERG's.
- Let's imagine the price of ERG is still NOW 1$.
- Alice has a call option 11.40$ in ERG (minus the exchange fee)
#  SigmaUSD (Stablecoin) Simplified
> SigmaUSD represents a call option on the dollar value of ERG held in reserve. 
{.is-success}

SigmaUSD uses Ergo's oracle pools infrastructure to calculate and adjust the current ERG/USD exchange rate. Reserve always backs sigma USD. The price ERG/USD floats (up/down) as users trade ERG.


**BASIC OVERVIEW**
- Bobs has 20 SigmaUSD that represents 20 USD value in ERG.
- These ERG's are held in Reserve.
- This 20$ of value is backed by reserves of at least
- (4x1)(80$ of ERG)(40 ERG @ $2)
- Bob at 2$ Bob can Redeem his 20 SigmaUSD for 10 ERG (minus the exchange fee)

**ERG/USD VALUE DROPS**
- Let us imagine the price of ERG drops from $2 to $1.
- Bobs 20$ of value is backed by at least
- (4x1)(80$ of ERG)(80 ERG @ $1)
- Bob can call 20 ERG (minus the exchange fee)

**ERG/USD VALUE INCREASES**
- Let us imagine the price of ERG increases from $2 to $4.
- Bobs $20 of value is backed by at least
- (4x1)(80$ of ERG)(20 ERG @ $4)
- Bob can call 5 ERG (minus the exchange fee)



# Longterm framework of SigmaUSD.
- SigmaUSD is an essential building block for a functioning DeFi System.  
- The focus for ERG now shifts to building on the foundation it has set. 
- Gateways, Dex's, Liquidity Pools, LETS systems. It is time to build use and utility. 
- The importance and significance of stable value cannot be overstated. 
- This is critical to the long-term prosperity of the Ergo Network and is important to understand. 

## Mining Incentives
> SigmaUSD offers a unique way for miners to create the base infrastructure for a robust DEFI system.
{.is-info}

Miners that maintain the network are the lifeblood of a robust POW system. A decentralised system will have a variety of actors that allow the system to grow. It is essential to consider the proper incentives to serve the needs of the community. Ergo is built on solid technological foundations; the decentralised financial market is made with historical foundations in mind.

Traditionally central banks held gold as reserves that backed currency. The currency was used as a stable medium of exchange throughout economies. When stable or backed by assets, this system of banking allowed commerce and growth.

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

## What is a stablecoin? 

> It is a derivate product. This derivative intends to create a way to stabilise volatility. 
{.is-info}

Price stability is a critical part of finance; without price stability, it becomes difficult to create long-term financial products modellings. Investment takes risk; a good business, whether on-chain or off, requires modelling and forecasting to estimate profitability. 

The crypto space, by nature is highly volatile. SigmaUSD and SigmaRSV are mechanisms to create stable value. Stable value is the foundation for a prosperous economy. 

Derivatives were created to minimise volatility when trading in foreign currencies. 

In a globalised economy, the shift in purchasing power of one currency vs another can be a highly destructive force. Instability disrupts trade and destroys business models. 

Stability comes at a cost. Instability in price is often added as a premium, sometimes a price premium, and other times an interest premium. 

The cost of SigmaUSD is the current USD value of ERG plus a 2.5% fee. 

This is a low premium, 2.5%. 

What is your current interest rate? What is the rate at which a bank will collateralise an asset you hold and offer a loan?

Very few have access to this low of a premium in the global economy, and the bank may not be offering liquidity with little to no reserve.

SigmaUSD allows anyone who owns ERG to collateralise their ERG and create liquid value. What does this mean?

The long-term goal will be to create use cases for this stablecoin that offers a return beyond this 2.5% fee. 

## Why?

> When Dapps and use/utility are in place that supersedes this 2.5% fee, magic happens. 
{.is-info}

A user can take their ERG, create SigmaUSD, then use that to create a return greater than the 2.5% cost of stability. The majority of business models rely on stability and price/risk prediction rather than asset speculation. 

SigmaUSD is not just an opportunity to take a short position on ERG. Rather it is a way to use your reserve value to generate yield. As Defi on Ergo delivers additional gateways, decentralised exchanges, or ergo swap liquidity pools, it allows growth opportunity for this stable value.No economy can function properly with high price volatility. A stable, robust decentralised economy requires a stable and robust mechanism currency. Ideally, a currency that is backed by a reserve asset to ensure its value.  

Once the 2.5% cost of stability is overcome, the dynamic of the SigmaRSV will change dramatically. Users have an incentive to continually mint/redeem SigmaUSD. Perhaps the value of ERG will go up, and a user may have missed some price appreciation; however, if they overcame the 2.5% threshold, the user had a net USD gain. 

Using stable value as the medium to invest and overcoming the 2.5% threshold generates returns. This transforms a short into a way to create value from stability.   

**Imagine the following scenarios.**
- A User chooses stability for a 2.5% premium. 
- Even if the price of ERG appreciates, and the user has the capacity to net again. It is true, they will have less redeemable ERG, but growth is growth. They end with a larger position in USD. 
- Perhaps ERG's value goes down; the stable value is used to create a net USD gain. Upon redemption, the stable value can be redeemed for a larger ERG position. Not only did they grow their position in USD, but they grew their position in ERG as well. 
- When SigmaUSD becomes a pathway of generative value beyond a short, it incentivises users to interact with the AgeUSD protocol on ERG. 
- The result of this will be a healthy reserve system that nets growth through interaction and exchange.

At this point, expect appreciation in SigmaRSV. Expect the treasury to grow. 

This is the major barrier to overcome, the 2.5% fee. 

All things being equal, this is a very low barrier to success. 
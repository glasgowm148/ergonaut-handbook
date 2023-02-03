---
title: TokenJay
description: open-source tool to exchange or burn Ergo assets/native tokens
published: true
date: 2023-02-03T19:22:40.585Z
tags: 
editor: markdown
dateCreated: 2022-09-14T23:34:20.515Z
---

# TokenJay
## Your place to go when dealing with tokens on Ergo platform
TokenJay's applications are open, fully documented and for everyone to use.

You need an ErgoPay compatible Wallet Application at hand.

- https://tokenjay.app/app/

TokenJay created by Benjamin Schulte aka [MrStahlfelge](https://github.com/MrStahlfelge). 


______
### Available tools on TokenJay:
**P2P Escrow**

Trade tokens person to person, trustless and decentralized with TokenJay's open P2P Escrow service.

The open P2P Escrow service is a smart contract that enables trustless, person-to-person (P2P), private sales on the Ergo blockchain for a small fee. The contract accepts Ergo tokens, such as a non-fungible token (NFT), 100 SigUSD, or other token(s) from the seller. Once in the contract, only a defined buyer sending a defined amount of ERG can access the token(s). If this happens, the contract sends the NFT, SigUSD or other token(s) to the buyer and the ERG to the seller. The seller can cancel the contract at any time before the exchange is made. To use:

1. Go to http://tokenjay.app
2. Connect wallet, by scanning QR code
3. Go to Your Token Sales
4. Click Start New Sale.
5. Select the vesting key from your wallet.
6. Put in buyer address.
7. Put in price buyer should pay. $ per SPF token, converted into Erg
8. Click Sell Token.
9. Sign transaction.

When transaction confirms, buyer can buy via tokenjay, it will show under P2P Escrow offers. Buyer needs to check token and minting transaction to confirm it is authentic. If an Ergopad vesting key, they can checking the tokenid in the verifier API:

https://api.ergopad.io/vesting/vestedWithKey/tokenid

This will return whether it is a real key, the token type and number of tokens. If it checks out, then they click Buy and sign the transaction.

When transaction goes through, Erg is sent to seller, key is sent to buyer, contract takes a small fee.

- https://tokenjay.app/escrow.html

**SigUSD and SigRSV** 

Convert ERG into SigUSD and SigRSV, directly with the bank and in a single transaction.
- https://tokenjay.app/ageusd.html

 **Utilities**

Token Burner- Burn unwanted NFTs and tokens.


- https://tokenjay.app/app/#burntoken

______
![tokenjay_mobilewallet_screenshot.png](/ergodapps/tokenjay_mobilewallet_screenshot.png)

🔼 TokenJay in mobile wallet 
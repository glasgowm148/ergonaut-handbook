---
title: Tip Bot
description: 
published: true
date: 2022-01-08T12:03:43.226Z
tags: 
editor: markdown
dateCreated: 2022-01-08T12:03:43.226Z
---

# Tip Bot

Supported Platforms
- Reddit
- Discord
- Telegram
- Twitter

Supported coins/tokens:
- Erg
- SigUSD
- SigRSV
- COMET
- Erdoge
- Ergold
- Kushti

You can restore the same seed in each instance, and use the same tip wallet across all platforms. 

## Getting Started

**First off. This is a bot that runs on a server managed by me (u/Luivatra). It is not unhackable (nothing is). Do not use this as a main wallet!**


### Reddit

1. Send a [private message](https://www.reddit.com/message/compose/?to=ErgoTipperBot&subject=BotTalk&message=!start) (**not chat!**) to u/ErgoTipperBot with the text: !start

2. Once the wallet is created, send a pm with !address to show your tip address

3. Copy your tip address and open your Yoroi wallet.

4. Click the send tab and transfer some ERG's to the tip wallet address. (Any transaction requires at least 0.001 erg in fees, on top of that funds in utxo are stored in a box. Each box needs to have a small amount of erg in them. So on the tip bot a token tip will require 0.00115 erg)

5. If you want to tip a token like Kushti for example, transfer the token to the same tip wallet address. 

6. Once the transactions are sent (~ 2 minutes), send a PM to u/ErgoTipperBot: !balance

7. Your balance should look like this:

| token  | amount |
|--------|:-------|
| Erg    | 0.1    |
| Kushti | 100    |

8. You are good to go! In one of the subreddits where u/ErgoTipperBot is activated write a comment to the person you want to tip with:
!tip <amount> <token> <any remaining text will be stored in the transaction database so you can both view it later>


Bot commands:

- In comments:
    - !tiphelp: Show this message
    - !tip <amount> <token> <any remaining text will be stored in the transaction database so you can both view it later>: tip the person you reply to
- In PM:
    - [!start](https://www.reddit.com/message/compose/?to=ErgoTipperBot&subject=BotTalk&message=!start): Initialize a tip wallet
    - [!changepw <currentPassword> <newPassword>](https://www.reddit.com/message/compose/?to=ErgoTipperBot&subject=BotTalk&message=!changepw%20%3CcurrentPassword%3E%20%3CnewPassword%3E): Change tip wallet pw
    - [!address](https://www.reddit.com/message/compose/?to=ErgoTipperBot&subject=BotTalk&message=!address): Show tip wallet address
    - [!seed <password>](https://www.reddit.com/message/compose/?to=ErgoTipperBot&subject=BotTalk&message=!seed%20%3Cpassword%3E): Show tip wallet seed phrase
    - [!balance](https://www.reddit.com/message/compose/?to=ErgoTipperBot&subject=BotTalk&message=!balance): Show tip wallet balance
    - [!restore <password> <seed phrase>](https://www.reddit.com/message/compose/?to=ErgoTipperBot&subject=BotTalk&message=!restore%20%3Cpassword%3E%20%3Cseed%20phrase%3E): Restore an existing wallet to be used as your tip wallet (use this to use the same wallet across Discord & Reddit)





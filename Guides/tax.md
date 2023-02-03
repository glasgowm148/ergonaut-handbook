---
title: Tax
description: 
published: true
date: 2023-02-03T19:36:09.936Z
tags: 
editor: markdown
dateCreated: 2022-03-24T14:38:12.122Z
---


# Formatting for Taxes using Koinly

Anyone struggling with Ergo taxes, it is possible to get Koinly to accept a csv and accurately represent everything. Here's how:
 
1. Retore wallet in SAFEW
2. Export .csv
3. Arrange first row with the following headings: date, sent amount, sent currency, received amount, received currency, fee amount, fee currency, txn hash (most of this is done, just move a couple around and create collumns for received
4. Cut and paste all positive values from the sent amount column and the sent currency (formerly 'balance') into the received amount and received currency collumns
5. Remove the '-' sign from the sent amount collumn so that all values are positive
6. Check for unrecognized currencies in the spreadsheet, some may be left blank. I just looked at SAFEW for this. If it was LP, I created a name that was consistent across those txns. If it was something dumb like spicy oatmeal, I just deleted those rows.

Edit in Google Sheets, then downloaded as .csv and uploaded to Koinly.

A complicated wallet can like 30 min, but most should be easy.

## Python Tool

There is also a Python tool to format transactions into .csv for Koinly.
https://github.com/crystoll/export-erg-transactions

# UK Tax

**Resources**

- [UK Tax Guide](https://recap.io/guides/uk-tax-full)
	- [HMRC: cryptoassets for individuals](https://www.gov.uk/government/publications/tax-on-cryptoassets/cryptoassets-for-individuals)
- [Penalties](https://www.litrg.org.uk/tax-guides/tax-basics/enquiries-penalties-appeals-complaints-and-debt/tax-penalties)
- [Tax Calculator](https://www.moneysavingexpert.com/tax-calculator/)


## Trading or Investing?

If you are treated as "trading" for UK tax purposes then you will be subject to Income Tax rather than CGT but HMRC guidance does state this would be in "exceptional circumstances" but you need to look at it on a case by case basis and look at previous guidance/case law, etc [1](https://www.gov.uk/hmrc-internal-manuals/cryptoassets-manual/crypto20250)

- [£1k "trading allowance"](https://www.gov.uk/guidance/tax-free-allowances-on-property-and-trading-income) 

## Gambling

Gambling winnings aren't taxable to income tax or capital gains tax. That sounds generous, but really its because people are more likely to lose than win so its really for exempting the losses, with the Exchequer "taking the hit" on the tax on winnings. 

There's a certain similarity between a gambling game making use of skill, such as poker, and a battle card game. Use the HMRC guidance[1](https://www.gov.uk/hmrc-internal-manuals/business-income-manual/bim22017) to conclude that you aren't trading. That means the basic position is true for you and you aren't taxable on your winnings.

> HMRC does not consider the buying and selling of cryptoassets to be the same as gambling. The term ‘gambling’ is not defined in the Income Tax or Corporation Tax Acts, or in the Taxation of Chargeable Gains Act 1992. Whether a transaction can be characterised as betting or gambling is a question of fact. It will be down to the caseworker to consider the particular facts of any transaction involving cryptoassets and conclude whether that transaction had the character of betting or gambling. Where a customer considers that their transactions involving cryptoassets amounted to gambling please make a referral following the process at CRYPTO100500.[1](https://www.gov.uk/hmrc-internal-manuals/cryptoassets-manual/crypto10450)


It's basically saying they don't consider buying and selling crypto to be gambling and therefore it is taxable but if you are genuinely gambling then they have the discretion to review it on a case by case basis and make a decision

But we don't know what their process is to make that decision


## Capital Losses

You ideally should report losses on Self Assessment return if you complete one. But for reporting capital losses you actually have **four years** from the end of the tax year that they arise in to report them.

Tax year runs **6th April to 5th April**. So if you have losses in period 6th April 2018 to 5th April 2019 then you have up to 5th April 2023 to report them.

Once reported they become usable in the tax year they arose. If you can't deduct them against gains in that year then you can carry them forward until you have a tax year in which you have gains.


## Charity


- [CRYPTO22100 - Cryptoassets for individuals: Capital Gains Tax: what is a disposal](https://www.gov.uk/hmrc-internal-manuals/cryptoassets-manual/crypto22100)
- [CG66621 - Reliefs: Capital Gains Tax and Gifts: Exemptions and No Gain/No Loss: Calculation for Gifts to Charities](https://www.gov.uk/hmrc-internal-manuals/capital-gains-manual/cg66621 )

## Income


> **Crypto capital losses cannot be set against crypto income profits.** You can end up with a large income tax liability and a large capital loss and cannot offset the losses and have no money to pay the tax with 
{.is-danger}

If you receive 1000 tokens and their spot price at that time is £1, your pre-tax income excluding any other factor would be £1000. What isn't clear, and I cannot offer much advice on this, is whether you are self employed or an employee of this project, as it will fundamentally differ how you pay tax otherwise. 

The tokens once you have them unconditionally are then at the whim of its own value; if it goes up there is a capital gain, if it goes down there is a capital loss, which is crystallised when you sell your tokens


**Example: Receiving volatile non-cash assets as income**

1. Get paid 1000 tokens worth £1/each
2. Price goes to 100/token for three months and back to £1
- You now have £3000 worth of tokens, but an income tax liability of £300,000
- You cannot offset any capital losses against your income tax liability but only against future capital gains.   

### As a Ltd

There are scenarios where using a Ltd can bring advantages profit wise -- with a Ltd you can offset income against capital losses during the same year. If you make income via interest or mining, a Ltd can get a 0 tax bill for the year if you happen to make capital losses
 
 
**Sideways Loss Relief**

> You can set the loss from your self-employment against capital gains in the same tax year in which you made the loss and/or the tax year prior to that in which you made the loss, but you must offset the loss against any other income in the tax year first (before setting it off against capital gains). So, you can only set a self-employment loss against a capital gain to the extent the amount of the loss exceeds the other income in the tax year.[1](https://www.litrg.org.uk/tax-guides/self-employment/working-out-profits-losses-and-capital-allowances/what-if-i-make-loss)

- [CRYPTO42100 - Cryptoassets for businesses: Income Tax: exchange tokens provided in the form of Readily Convertible Assets (RCAs)]( https://www.gov.uk/hmrc-internal-manuals/cryptoassets-manual/crypto42100)

> The business can treat income as received and expenses as paid at the date of its choosing, as long as the treatment is consistent. For example, an expense may be paid when a card payment is made, or on the date that entry is shown on the bank statement.

- [BIM70005 - Cash basis: overview](https://www.gov.uk/hmrc-internal-manuals/business-income-manual/bim70005)


**Using SigmaUSD**

1. Paid £10k in crypto
2. Turn into £10 SigmaUSD
3. Price halves
3. Redeem double the erg (still worth £10k)
- £10k taxable income.
- ERG with a base cost of £10k. No gain/loss until disposed of.


**Investing in another token**

1. Paid 1000 erg = £10k
2. Price halves
3. sell 1000 erg for £5k worth of some other token
4. token does a 4x in value and is worth £20k
- £10k taxable income.
- £5k capital loss on ERG.
- No gain/loss on other token unless sold. 
- If sold/exchanged when worth £20k, then £15k capital gain. This would then net against the ERG loss so be a net £10k capital gain for the tax year.

## NFTs

- Minting NFT - acquisition at cost of eth gas fee (with a disposal of the eth used for the fee)
- Stealing NFT - acquisition at £nil cost. I suppose it might be S22 disposal of rights but that seems tenuous
- NFT dies - S24(1) TCGA 1992 disposal
- NFT stolen - disposal for £nil consideration (I can't see how it could be a S17(1)(a) TCGA 1992 situation)


## Staking/Lending

The new HMRC defi guidance has highlighted that some token rewards received for staking/lending type activities may be capital in nature rather than revenue (income). Let’s say it is clear there is no transfer of beneficial ownership upon entering the yield farming activity. Would there still need to be a CGT calc done to tax the estimated Marren v Ingles capital return upon entry? So if on entry the estimated capital return is £100, that is subject to CGT at the time of staking/lending? I think the HMRC examples only seem to mention a capital return where there is also a transfer of beneficial ownership.

Hmm, a curious scenario. I think the Marren v Ingles right would be a "capital sum derived from an asset", the asset being the cryptoassets you still own but that you are using for yield farming. In that situation section 22 TCGA 1992, would treat you as making a part disposal of the cryptoassets.

## Airdropped governance tokens

HMRC has guidance on airdrops at https://www.gov.uk/hmrc-internal-manuals/cryptoassets-manual/crypto21250. Their position is that airdrops that are provided in return for, or in expectation of, a service are subject to income tax. If there's no expectation of a service then income tax doesn't apply.

Are you receiving the governance tokens in return for doing something? If not then income tax won't apply.

## Staking governance tokens

HMRC has guidance on staking at https://www.gov.uk/hmrc-internal-manuals/cryptoassets-manual/crypto21200. Their position is that any return on staking is taxable to income tax. They expect the income tax charge roll normally arise under miscellaneous income, but that there might be a trade depending on the facts.


## Liquidity pools for in game currency

HMRC doesn't yet have any guidance on liquidity pools. The safe assumption is that HMRC will seek to tax returns to income tax, much the way that HMRC taxes interest on loans to income tax.

There are still a tricky questions. When does the income tax charge arise? With interest the tax charge occurs when the interest is made available, which tends to monthly. Liquidity pools may pay the returns daily or even more frequently than that. Does that mean having to calculate the DEC accumulated each time, it's sterling value each time and then the tax on that? Sadly the answer from HMRC is probably going to "yes".

Then there's the issue of many tokens having a fluctuating value during the day. This isn't unique to crypto. The value of shares and currency will fluctuate in a day. For this reason HMRC are willing to accept the daily value (which tends to be the midpoint of the daily min and max) rather than the value at any particular time in the day. We can hope that HMRC will take the same approach with crypto, although it does then require someone to work out that daily value. For shares that is normally the share exchange, eg the FTSE. Maybe a site such as Google might suffice for crypto. Time will tell
Going about what? Establishing the price you purchased it for?


## Changing the law

Even the HMRC advice is based on opinions. Everyone is drawing conclusions from existing legal principles. That's how the law in the UK tends to work - the courts see a situation and establish how that should be treated. That treatment then continues until either a higher court overturns the existing treatment, the courts distinguish a similar but different situation, or the law is changed by legislation.

Imagine if tax legislation had been introduced in 2018. It would have covered basic transactions, forks, airdrops and ICOs because they were the big thing at the time. It wouldn't cover DeFi or NFTs, even though both existed at the time, because they were niche and so a mere curiosity. So then you'd need more legislation in 2019, 2020, 2021. What's the big thing(s) in 2022? Will it be the metaverse, fan tokens, reflections, cashback? Maybe something that doesn't even exist yet.

You might think that it would be better to have some basic tax legislation for crypto and just to apply that to the new things. But that's barely different to what's going on now with the tax system anyway. Legislation can give rise to odd outcomes where it covers a situation that it isn't designed for. Using principles rather than legislation at least gives some scope for seeking a pragmatic answer.

I'm afraid until the sector starts to stabilise then tax legislation is unlikely. We'll have to keep providing our opinions and hope for some cases to go through the courts to start putting those opinions on firmer footing.



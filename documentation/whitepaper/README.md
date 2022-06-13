# Whitepaper

## Abstract

Unbound Finance is building the next money lego through unlocking the TVL (Total Value Locked) within the DeFi system with a view to augment the utility of Liquidity Provider (LP) tokens, making it a more efficient yield generating tool. \


The whitepaper gives a brief summary of the Unbound project.

## Introduction

Unbound is a decentralized cross-chain liquidity protocol that is building the derivative layer of Automated Market Makers (AMM). The intent of Unbound is to build products that are both native and composable to the DeFi ecosystem. These include

* Synthetic Assets including a Stablecoin(UND), uETH,etc
* AMM pools that are cross derived from multiple AMMs
* Oracle Price Feeds based on free markets and path independent value discovery.
* Building financial instruments for compounding yields and margin trades

Unbound protocol is building a management layer over the existing AMMs by locking up LPT to mint synthetic assets that further reinforces liquidity in AMMs and Defi, unlocking liquidity from existing AMM Liquidity Pools. The initial set of product Unbound has been built to include decentralized, cross-chain stablecoin called UND.

Unbound has created a robust architecture that does not require a Liquidation Engine. A combination of collateral ratio, risk management through selected stablecoin-ERC20 LPT pairs, and SAFU fund ensures a support system that is a lot more resilient than traditional crypto assets under similar circumstances. This is a huge shift from the existing lending landscape.

### What is DeFi?

‌Decentralized Finance (DeFi) is a financial system built on decentralized assets. The DeFi ecosystem comprises lending and borrowing, decentralized exchanges, and derivatives trading among other facilities. \


The DeFi market consists of many innovations such as:\


* Lending Platforms - Compound, Aave, dYdX, Oasis, MakerDAO, Dharma etc.
* Decentralized Exchanges (DEX) - Uniswap, EtherDelta, Bancor.
* Assets – Digital assets such as WBTC, RenBTC etc.
* Derivatives - Dai, Synthetix etc.
* Payments – Platforms such as Flexa (Ethereum) and the Lightning Network (Bitcoin).

In October 2020, the total value locked in DeFi in USD is $10.71 Bn. Uniswap alone dominates 23% of the market share.&#x20;

![](https://lh4.googleusercontent.com/kLxt5RTIWFp4Ai2nW6T17iZXHJByYrUMPOLzXMZ8jMogFjHbEQDwzJzo69ujwP4Uuq9l3yvIfQajxRJQlzjXSL5eECbty1kWT0-WhQ8X3SyKSO6z6woqQ81rv06PdkU5Gfwvtylz)

[Defi Pulse](https://defipulse.com/)\


### Automated Market Makers (AMM)

‌AMM is an implementation of Decentralized Exchanges (DEXs). AMMs replace the existing exchange order-books with a permissionless liquidity pool run by algorithms. In DeFi, the constant flow of liquidity is handled by AMMs. Smart contracts lock tokens in order to provide liquidity which enables token pair exchanges. In return, the users, also called Liquidity Providers, are issued an LPT (Liquidity Pool Token) that represents the value they put into the Liquidity Pool.&#x20;

## Unbound: A Derivative for AMMs

DeFi is evolving with various derivative layers and AMMs are building new smart contract based legos. Unbound is a DeFi platform that creates a treasury layer on top of existing AMM platforms by using LPT’s as a collateral, which is a decentralized receipt of the user’s funds in an AMM pool.  \


Unbound provides the first-ever debt-free liquidity provision system! The platform provides liquidity to AMM LPTs and issues a Stablecoin (UND) in the form of a minted token. The platform unlocks the LPTs once the UND is returned, irrespective of time. The user is never at risk given that Unbound does not have a Liquidation Engine!\


![](../../.gitbook/assets/group-121-1-.png)

1. Unlock LPT Liquidity: LPTs are the ideal collateral. They are great for funding but unsuitable for trading. Unbound will collateralize LPTs via smart contracts, which provide additional liquidity, without compromising on security.
2. Mint Stablecoin by locking LPTs: Contracts will lock LPTs and mint a stablecoin (UND).
3. No Liquidation Engine for LargeCap Pairs(Eth/Dai,USDT/USDC,etc) : Unbound does not have a liquidation engine. The smart contracts unlock collaterals whenever the minted UND is returned. What this imply is that when you mint UNDs, this does not create a debt position where:
   1. Users do not lose any collateral amount
   2. Unbound does not charge any penalty amount if the value of collateral goes below a certain amount.
4. SAFU fund: In case of an exceptionally steep decline in collateral value, the SAFU fund is there to absorb some or all of the losses without liquidating the user collateral. More details in the following sections.

## Core Features

‌Unbound provides three main services in the form of fully automated Smart Contracts that do not require any third party intervention. The Smart Contracts make sure that the LPT pool is valid before a transaction can be created.

### ‌Minting

‌UND tokens and other synthetic assets are minted when users provide their LPT as collateral. The UND token represents a stablecoin pegged to the value of USD. Once users have their UND, they can use the funds immediately. Unbound will initially support LPTs from various AMMs such as Uniswap, Balancer, Mooniswap, Curve, Kyber, and Bancor, with others to follow.&#x20;

The Loan-to-Value (LTV) ratio is the percentage of funds that users can mint against their collateral. This ratio is variable. For example if it’s set at 50%, for every $100 worth of LPT token deposited, users can mint up to 50 UND. There is a minting fee charged to the user. This minting fee acts helps to provide stability for the ecosystem and will remain variable to help UND maintain its dollar peg.&#x20;

‌The UND minting terminology:

UND = Unbound Stablecoin&#x20;

LPT = Liquidity Pool Token&#x20;

LTV = Loan-to-Value Percentage&#x20;

Minted UND = LTV x USD value of LPT&#x20;

mFee = \[Minting Fee % ] X \[ Minted UND]

Minted UND to the USER = Minted UND -  mFee\


![](../../.gitbook/assets/group-130.png)

### Unlocking

‌When users pay back their minted funds (including the minting fees), the UND is burnt during the unlocking process. This takes the minted UND out of circulation and in return the user gets back their collateralized LPT. There will be no other additional fees charged to users when they unlock their LPT.

‌Unbound smart contracts are perpetual, meaning they don't have a maturity date on the money that has been minted, therefore there is no deadline for repayment of funds and users can continue to earn from their LPT.

Unlocked LPT = Returning Minted UND

![](../../.gitbook/assets/group-136.png)

###

## Liquidation Free Liquidity

Liquidation Free Liquidity is a 2 step process

1. Lockup LPT tokens from large market cap pairs (Eth/Dai,ETH/USDT,DAI/USDT, USDT/USDC, etc)
2. A LTV ratio that does not risk the collateral even during steep corrections.&#x20;
3. Maintain a SAFU Fund that with time can act as an insurance fund.&#x20;

The most important part of using LPT tokens as a means of collateral is working out the impermanent or divergence loss that can erode the value of the collateral. To make it clearer, we would link the impairment loss in terms of the correction that the erc20 token will undergo in order to derive a breakeven price of the erc20 token with respect to the LTV.

### Deducing the formula for Impermanent loss&#x20;

#### Case 1 – HODL

A user holds e0 ETH and u0UND. He has equal values of the two (measured in ETH, or equivalently in any other currency). The initial price therefore is given by: p0=(e0/u0)&#x20;

And the initial value of the holdings (measured in ETH) is given by:

![](../../.gitbook/assets/screenshot-2020-11-08-at-5.48.58-pm.png)

At some time in the future, the price has changed to p1, but the number of each token he holds (e0 and u0) is unchanged. So his holdings are now worth:

![](../../.gitbook/assets/screenshot-2020-11-08-at-5.49.07-pm.png)

#### Case 2 - provide liquidity to Uniswap

Now, if he supplies his tokens to Uniswap, the constant product formula will work out how much ETH and UND he can claim from the liquidity pools, e1 and u1. In Uniswap, the ratio of the two pools is equal to the price of the two tokens:

![](../../.gitbook/assets/screenshot-2020-11-08-at-5.50.21-pm.png)

So when the price changes to p1, we know that:

![](../../.gitbook/assets/screenshot-2020-11-08-at-5.53.52-pm.png)

And from the constant product rule (excluding fees):

![](../../.gitbook/assets/screenshot-2020-11-08-at-5.50.41-pm.png)

Combining these two we have:

![](../../.gitbook/assets/screenshot-2020-11-08-at-5.51.01-pm.png)

So the value of the liquidity he can now withdraw from Uniswap is:

![](../../.gitbook/assets/screenshot-2020-11-08-at-5.51.09-pm.png)

\
**Impermanent loss**\
****We then find the difference between _`VH`_ (the value from the hodl strategy) with VU (the value from the Uniswap strategy) to work out the difference _`VD`_ . It's more useful to find this as a fraction of _`VH`_ so we divide both sides by _`VH`_.

![](../../.gitbook/assets/screenshot-2020-11-08-at-5.58.00-pm.png)

To reframe this in terms of the price ratio PR(price ratio) = (p1/p0), we divide the top and bottom of the fraction by e0:

![](../../.gitbook/assets/screenshot-2020-11-08-at-5.58.09-pm.png)

**Note**

The value of `(VD/VH)`will always be ≤ 0, showing that there is always a Impermanent loss  unless `(p1/ p0)=1, i.e. p1=p0)`\


The above was also used by uniswap for [understanding returns on their ecosystem](https://uniswap.org/docs/v2/advanced-topics/understanding-returns/).\


### Deducing Unbound breakeven formula or Meeth’s Formula

![](../../.gitbook/assets/screenshot-2020-11-07-at-2.29.59-pm.png)

![](../../.gitbook/assets/screenshot-2020-11-07-at-8.00.08-pm.png)

![](../../.gitbook/assets/screenshot-2020-11-07-at-8.00.20-pm.png)

### Meeth’s Formula

![](../../.gitbook/assets/screenshot-2020-11-10-at-3.27.33-pm.png)

Note: We have added the fees earned by LPT tokens by using the volume numbers disclosed by Uniswap.\


This formula is the foundation of our algorithm. To make things easier, we have created a [calculator](https://testnet.unbound.finance/calculator/) that will process the Maths in the backend.\


For an ETH-DAI pair with an LTV of 50%, our net break-even price percentage is at - 74.9684%\


![](../../.gitbook/assets/screenshot-2020-11-10-at-1.24.30-pm.png)

This means that in the above example with the current ETH price at $444.73, ETH would have to correct all the way to around $111 (-75%) for the underlying collateral to become 100% collateralized.&#x20;

You would also see Duration(days) in the [calculator](https://app.unbound.finance/calculator). This signifies the time it takes for the erc20 to decline in price and is required so that the fees that the LPT tokens earn can be calculated. These fees that are earned are then subtracted from Eth Break Even Price to get the Net BreakEven Price.&#x20;



## Tokens

The Unbound protocol is a dual token ecosystem. It uses UND as a stablecoin and UNB as a governance token.

**‌UND - The End Of Centralized Stablecoins!**

The UND is a stablecoin that is pegged to USD and collateralized by LPT (Liquidity Pool Tokens). The value of UND minted is based on the value of the deposited LPT. The amount of UND minted at the time the LPT was deposited is the amount that the user must pay back in order to get their original LPT. Minted UND will be burned once deposited in the Unlock contract before the original collateral is returned to the user. Arbitrageurs in AMM pools ensure that the Dollar peg is maintained.

‌**UNB**

UNB is used for protocol governance. It encourages participation from the token holders by way of decision making to resolve issues. Token holders will be able to vote for policy on proposed changes and implementations to better serve the community and increase the efficiency of the protocol. More details on governance is covered in the upcoming sections.

A perpetual inflation rate of 4% per year will start after 2 years, ensuring continued participation and contribution to Unbound at the expense of passive UNB holders.

## Tokenomics\*

TGE: 14/12/21

Total Supply: 10 Billion

Chain Supported: ETH & BEP20

* UNB ERC20 Token Address: [0x8db253a1943dddf1af9bcf8706ac9a0ce939d922](https://etherscan.io/address/0x8db253a1943dddf1af9bcf8706ac9a0ce939d922)
* UNB BEP20 Token Address: [0x301af3eff0c904dc5ddd06faa808f653474f7fcc](https://bscscan.com/address/0x301af3eff0c904dc5ddd06faa808f653474f7fcc)



![](<../../.gitbook/assets/Tokenomics pie chart-01.jpg>)



### Vesting Schedule

| Investment Round            | Allocation Percentage	 | Token Release Schedule                                                          |
| --------------------------- | ---------------------- | ------------------------------------------------------------------------------- |
| Friends & Family Round      | 6.14%                  | 10% on TGE, rest vested linearly over 34 months with a 6 months cliff from TGE. |
| Early Backers Round         | 5.32%                  | 10% on TGE, rest vested linearly over 27 months with a 6 months cliff from TGE. |
| Seed/Private/Strategy Round | 12.43%                 | 10% on TGE, rest vested linearly over 18 months with a 6 months cliff from TGE  |
| Institution/Venture Round   | 5.07%                  | 10% on TGE, rest vested linearly over 27 months with a 6 months cliff from TGE. |
| Public (IDO)                | 0.37%                  | <p>30% on TGE, 30% after month 1, 40% after </p><p>month 2.</p>                 |
| Public (IEO)                | 0.67%                  | 100% on TGE.                                                                    |
| Treasury                    | 30%                    | 20% on TGE, rest vested linearly over 24 months with a 3 month cliff from TGE.  |
| Team                        | 25%                    | 0% on TGE, rest vested linearly over 42 months with a 6 months cliff from TGE.  |
| Foundation                  | 15%                    | At different stages of project development.                                     |

### Foundation & Investor Wallets Info

| Wallets                  | Address                                                                                                               | Allocated Tokens    |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------- | ------------------- |
| Unbound Investor Vesting | [0xc49Ca76EbFA713B90a60f5C1d55B35561e5FA528](https://etherscan.io/address/0xc49Ca76EbFA713B90a60f5C1d55B35561e5FA528) | 2896000000 (28.96%) |
| Unbound Team Vesting     | [0x0e3e039e4c8b68cda90ddbf9fddec7c1a1032202](https://etherscan.io/address/0x0e3e039e4c8b68cda90ddbf9fddec7c1a1032202) | 2500000000 (25%)    |
| Unbound Treasury Vesting | [0x9bBfa6d19d8BAec1D7a09781c84f1A0A7656B2Fd](https://etherscan.io/address/0x9bBfa6d19d8BAec1D7a09781c84f1A0A7656B2Fd) | 2400000000 (24%)    |
| Unbound Foundation       | [0x504Aaaa2c4a94cDF7E32333C665CEAa3cEf648fa](https://etherscan.io/address/0x504Aaaa2c4a94cDF7E32333C665CEAa3cEf648fa) | 1500000000 (15%)    |
| Unbound Treasury         | Currently in circulation.                                                                                             | 600000000 (6%)      |
| Public Sale (IDO+ IEO)   | Huobi, Kucoin, Polkastrater, Redkite and Gamefi.                                                                      | 104000000 (1.04%)   |

### Investor Vesting Addresses

| Type of Investor   | Address                                                                                                               |
| ------------------ | --------------------------------------------------------------------------------------------------------------------- |
| Friends and Family | [0x0d3891F52EAB019612FE5DF32E278b81D4af2DFA](https://etherscan.io/address/0x0d3891F52EAB019612FE5DF32E278b81D4af2DFA) |
| Early              | [0x3B4e5Be9C380bA7f0E8E88f98e9928d3e6Df96D0](https://etherscan.io/address/0x3B4e5Be9C380bA7f0E8E88f98e9928d3e6Df96D0) |
| Seed               | [0x80f666E786F3Bc862a0D7d762D3f7C7193a7681F](https://etherscan.io/address/0x80f666E786F3Bc862a0D7d762D3f7C7193a7681F) |
| Private            | [0x67b62a4427a6f1111b94193F96f3a81122f1FD5f](https://etherscan.io/address/0x67b62a4427a6f1111b94193F96f3a81122f1FD5f) |
| Institution        | [0xfB1dE6E1021a1E503f31aD42BD26891e68bb29c8](https://etherscan.io/address/0xfB1dE6E1021a1E503f31aD42BD26891e68bb29c8) |
| Venture            | [0x439f729e66022d1BA592b1E04Ad0804eB5Dfca35](https://etherscan.io/address/0x439f729e66022d1BA592b1E04Ad0804eB5Dfca35) |
| Strategic          | [0x107678C8EF64E8e8DAb40bFCcA6f8a1ebC82D99a](https://etherscan.io/address/0x107678C8EF64E8e8DAb40bFCcA6f8a1ebC82D99a) |

### Circulating Supply <a href="#circulating-supply" id="circulating-supply"></a>

| Time span       | Circulating supply                                      |
| --------------- | ------------------------------------------------------- |
| 0 to 3 months   | 9.74% (6% Treasury & 3.74% from Private & Public Sale). |
| 3 to 6 months\* | 12.73%(9% Treasury & 3.74% from Private & Public Sale). |
| 6 months +\*\*  | Linear vesting starts as described in the above table.  |

> \*Foundation Tokens have no fixed vesting schedule and would be unlocked for liquidity mining rewards and strategic fund raise . We would inform community before any type of unlock occurs.

> \*\* There will be an inflation of 4% after 2 years from TGE.

## Fee Distribution\*

‌The fees collected from minting will get distributed to SAFU fund, Team fund, and UND liquidity pool. Its allocation is not fixed and as the system becomes more autonomous, the portion allocated can go up or down as required.

a) SAFU Fund \
b) UND Liquidity Pool \
c) Team Fund

SAFU Fund and Liquidity Pools (Earn) are covered in the earlier sections.

**Team Fund**

‌Some portion of fees is distributed to team members to enable further development. This allocation is not fixed and is subject to change as required.

## Unbound Factory

The Factory Smart Contract is to support major LPTs which include Uniswap, Balancer, Mooniswap, Curve, Kyber, Bancor, and others in the pipeline.\


![](https://lh4.googleusercontent.com/lnUSkR8kiIHZoMRMZ2LJjAcW9zG3Q8RNh8E5M9rph7KBU12QRe4EowLDcWLE1XB8PuckMTzAeRymf5FMOoH\_f6hcvagWrDdDPno9kvkhdxXp4\_lTaiP9ehQrjPzygUICVnM8JOZF)

## Roadmap

![](https://lh6.googleusercontent.com/y9G4mKAAPHO\_y6A1sg1DWGeZV1iOhwzrXPltIdG6yA3jtqivC\_b88fJGKqTbxzcc3gUxqcp5V1RqdHh50YyxfqFkkQxlgaXI4q57JEDB04zwtNlkeSIeafj9ZAAulJLYuEoxyxXs)

## Governance

Unbound will implement a DAO in the coming days.

* The Unbound governance model enables UNB token holders to participate in policies and protocol decisions on the platform. The amount of UNB tokens that a user holds is proportional to their voting power on the platform.
* The voting power of a user gives them the right to participate in policy making, proposals, and to have a say in any future direction of the platform.
* The DAO (Decentralized Autonomous Organization) has Smart Contracts that form the backend of the platform.
* The DAO maintains the transaction records and rules that must be implemented on the blockchain for Unbound's protocols.
* Tokens allocated for the DAO are more for financing the platform since the Smart Contracts do not vote.
* The UNB tokens are stored by the DAO, and are released when new policies and improvement proposals from the community have been passed. These will be used to fund projects for the platform.

## Further Develop‌ments&#x20;

**Version 1**

Unbound’s goal is to become a DeFi treasury for LPT and increase liquidity for UND.

V1 primarily focuses on:

* Creating a first-ever debt-free liquidity provision system
* Unlocking liquidity from existing largecap AMM Pools for the UND stablecoin
* Producing fee-earning, non-tradeable collateral
* Implementing a SAFU fund

**Version 2**

Unbound will work towards a more autonomous organization for decentralized liquidity and earnings. This will allow users to explore different markets that provide the best yields on digital assets with the benefits of minimal risk liquidity provisioning.&#x20;

V2 will primarily focus on:

* Unbound Virtual AMM (vAMM): Unbound vAMM will introduce a Vault mechanism which will work autonomously, providing automatic liquidity algorithmically.
* Unbound Price Oracles: Unbound will develop an on-chain price oracle to query other Smart Contracts to find the latest and most accurate prices with the aim of minimizing the risk of losses to users.
* Unbound Liquidation Engine for volatile pairs: Unbound will introduce a liquidation engine solely for volatile pairs. When a certain token value falls below a threshold, the liquidation process will be initiated. Unbound’s community governance will decide which volatile assets will be subject to the liquidation protocols.

![](https://lh5.googleusercontent.com/aQLbSyYJ0vc6IxcskFi7cRmZdT0qSSQwpce2Qmy2i9oG764j\_7uGj3\_1lqHkhQ-8Ek27yJnoXFOEBNyHpCvZmsB8SDgVhqr8G5MVOnuutW7wu0bZqGrm1taJ994RWuNeSxcoLyP2)

## Conclusion

‌Unbound is the next logical step in the evolution of Decentralized Finance. The platform enables the unlocking of LPTs to be used as collateral for minting Unbound's UND stablecoin. UND, being a stablecoin, has unlimited use cases. The platform, importantly, does not have a liquidation engine which provides a much-needed protection against liquidation of user collateral caused by extreme market volatility. It also issues its native UNB token to users who are providing liquidity, granting them voting rights. These votes can be used to bring about changes and to have a say in the future direction of the Unbound platform.

## References

1. Uniswap: A Good Deal for Liquidity Providers? - [https://medium.com/@pintail/uniswap-a-good-deal-for-liquidity-providers-104c0b6816f2](https://medium.com/@pintail/uniswap-a-good-deal-for-liquidity-providers-104c0b6816f2)
2. DeFi Explained: Automated Market Makers - '[https://medium.com/multi-io/automated-market-makers-amm-breakdown-d3338f027230](https://medium.com/multi-io/automated-market-makers-amm-breakdown-d3338f027230)'
3. What Is DeFi - '[https://www.coindesk.com/what-is-defi](https://www.coindesk.com/what-is-defi)'
4. The Great Potential Of Decentralized Finance in 2020 - '[https://www.entrepreneur.com/article/353588](https://www.entrepreneur.com/article/353588)'
5. What Is Automated Market Making And Why Does It Matter - '[https://digitexfutures.com/blog/what-are-automated-market-makers-and-why-do-they-matter/](https://digitexfutures.com/blog/what-are-automated-market-makers-and-why-do-they-matter/)'
6. How Do Liquidity Pools Work? DeFi Explained - '[https://medium.com/@finematics/how-do-liquidity-pools-work-defi-explained-6d3418ea71fa](https://medium.com/@finematics/how-do-liquidity-pools-work-defi-explained-6d3418ea71fa)'
7. What Is ERC20 And What Does It Mean For Ethereum - '[https://www.investopedia.com/news/what-erc20-and-what-does-it-mean-ethereum/](https://www.investopedia.com/news/what-erc20-and-what-does-it-mean-ethereum/)'
8. Curve Finance Is Fixing Stablecoin Slippage on DeFi - '[https://cryptobriefing.com/curve-finance-fixing-stablecoin-slippage-defi/](https://cryptobriefing.com/curve-finance-fixing-stablecoin-slippage-defi/)'
9. Beginner’s Guide to (Getting Rekt by) Impermanent Loss - '[https://blog.bancor.network/beginners-guide-to-getting-rekt-by-impermanent-loss-7c9510cb2f22](https://blog.bancor.network/beginners-guide-to-getting-rekt-by-impermanent-loss-7c9510cb2f22)'
10. Constant Function Market Makers: DeFi’s “Zero to One” Innovation - ‘[https://medium.com/bollinger-investment-group/constant-function-market-makers-defis-zero-to-one-innovation-968f77022159](https://medium.com/bollinger-investment-group/constant-function-market-makers-defis-zero-to-one-innovation-968f77022159)’

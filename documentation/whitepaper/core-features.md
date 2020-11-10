# Core Features



## Core Features

‌Unbound provides three main services in the form of fully automated Smart Contracts that do not require any third party intervention. The Smart Contracts make sure that the LPT pool is valid before a transaction can be created.

### ‌Minting

‌UND tokens and other synthetic assets are minted when users provide their LPT as collateral. The UND token represents a stablecoin pegged to the value of USD. Once users have their UND, they can use the funds immediately. Unbound will initially support LPTs from various AMMs such as Uniswap, Balancer, Mooniswap, Curve, Kyber, and Bancor, with others to follow. 

The Loan-to-Value \(LTV\) ratio is the percentage of funds that users can mint against their collateral. This ratio is variable. For example if it’s set at 50%, for every $100 worth of LPT token deposited, users can mint up to 50 UND. There is a minting fee charged to the user. This minting fee acts helps to provide stability for the ecosystem and will remain variable to help UND maintain its dollar peg. 

‌The UND minting terminology:

UND = Unbound Stablecoin 

LPT = Liquidity Pool Token 

LTV = Loan-to-Value Percentage 

Minted UND = LTV x USD value of LPT 

mFee = \[Minting Fee % \] X \[ Minted UND\]

Minted UND to the USER = Minted UND -  mFee  


![](https://lh4.googleusercontent.com/Flqq8xp2NGN945mkDG_wImrbWpBCPg0hDxEIdxn2H-UifD6TgyrDCrHwmlwKP1Ndv2qgA7AlXcNCfwbqI6GygiMdCOvftXxWnfMSZJl3i0LXAyI4YPdghCi_2JHy0QQmFJcMRMd8)

### Unlocking

‌When users pay back their minted funds \(including the minting fees\), the UND is burnt during the unlocking process. This takes the minted UND out of circulation and in return the user gets back their collateralized LPT. There will be no other additional fees charged to users when they unlock their LPT.

‌Unbound smart contracts are perpetual, meaning they don't have a maturity date on the money that has been minted, therefore there is no deadline for repayment of funds and users can continue to earn from their LPT.

Unlocked LPT = Returning Minted UND

![](https://lh5.googleusercontent.com/25CX-9kvEWf0tTNj-s3Rp394uxuCYJXXKg9UyAdeslRb-iLqO5fL0SGh77-Y0UrpdMlvtS1_9YH_cXYdmDseEDyxXvRqJ_SthQYPbOnavp9HiRkm749RVvMoXD9OENIjssCxkoEZ)

### Earn     

Users can become Liquidity Providers for UND Pools. In return, UND is issued to users for providing that liquidity. ‌

* The Earn reward is over and above what a user will get in Uniswap
* The Earn reward is variable and is set to 40% of the Mint transaction fees in the initial phases. 


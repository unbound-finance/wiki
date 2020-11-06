# Mitigating Slippage And Impermanent Loss With Liquidity Incentives

One of the main problems on decentralized exchanges is the occurrence of _**slippage**_. This happens when the liquidity providers lose returns on their **LPT \(Liquidity Pool Tokens\)**  due to trading pair volatility. This is the nature of the cryptocurrency market, where price values fluctuate constantly. This also leads to **impermanent loss** to the participant due to price variations. When this happens, the liquidity provider may notice missing tokens from the pair they originally locked. It is called _impermanent_ because it can be a temporary loss of value, but if participants withdraw their tokens it can become a permanent loss.

If a liquidity provider contributes to a DAI/ETH 50/50 pool on Uniswap, they must provide the equivalent amount of each coin. When contributing to a Liquidity Pool with a 50/50 ratio, equal amount must be deposited for the token pairing.

For example, if DAI is valued at $1.00 and ETH is valued at $400. A participant wants to deposit $800 worth of ETH which is 2 ETH. They must also deposit an equal amount of DAI. 

**x = DAI = $1.00 -&gt; 800**

**y = ETH = $400 -&gt; 2**

The token pair is equal to 800 DAI and 2 ETH

**k = x  \***  _**y = 800 \***_  **2 = 1600**

We have a total of $1,600.00 in maket value in this token pairing.

Uniswap uses a protocol called the **Constant Product Market Maker** which maintains the correct ratio of tokens in a pool. If the price of ETH goes up to 450 on a certain exchange, it becomes an arbitrage opportunity to make a profit. 

Our constant product based on the token pair should remain at 1600. In order to keep the value of k constant, the ratios have to be adjusted. With ETH at 450, traders are going to add more DAI and take out some ETH. The difference with the price before and after arbitrage is the impermanent loss. If the liquidity provider decides not to withdraw their liquidity and the price of ETH returns to 400, it is an impermanent loss. If the liquidity provider decides to withdraw then that becomes a permanent loss because they have exited from the system.

### Liquidity Incentives

Liquidity incentives can mitigate impermanent loss as returns from the subsidy reduces the loss from volatility. This offers yields to anyone who contributes LPT to Unbound's Liquidity Pool. The digital asset pair in the LPT \(e.g. DAI/ETH\) is actually deposited in a Vault, where all collateral is stored. 

There are two ways that contributing liquidity can be incentivized. The first one is through the use of **Asset Inflation** and the other is through **Protocol Fees**. These are systems that offer incentives that mitigate losses from slippage and avoids impermanent loss by minimizing the risks. This is a best practice implementation for incentivizing participants with some level of certainty.

#### Asset Inflation

Inflationary assets can offset impermanent loss. This can be done through adding liquidity in the Unbound pool and claiming rewards. The inflation aims to attract more liquidity because of the profits that can be made by earning. As more Unbound tokens are created, it dis-incentivizes users from holding their tokens. It encourages incentives through more participation for users to be active on the platform. Token holders can also vote to adjust the protocols when it is necessary. However, the idea of an inflationary model is to reward participation in the ecosystem and earn.

As an example, let us say that minting of tokens has increased the supply relative to the market cap. A locked LPT does not have a fixed value. One participant may lock an LPT worth $500, while another can have $1,500,000. You get more tokens the more value your LPT is worth. As more participate in minting tokens the supply increases with no fixed cap. In terms of earnings, it can have a compounding effect as having more tokens is better.

#### Protocol Fees

There are revenues collected from fees on the platform for minting and unlocking LPT. These fees are deposited into a fund pool collected from transactions. Each transaction in the Unbound pool is charged a fee of 0.03 or 0.3%, which is then distributed among the token holders who stake Unbound tokens. Those who hold a higher stake can earn more per transaction.

Protocol fees can also increase due to demand. With the governance consensus mechanism, if the ecosystem is being overwhelmed by too many transactions, the fees can increase slightly with majority consensus among token holders who vote.

### Conclusion

Slippage and impermanent loss in DeFi is inevitable due to the volatility in the cryptocurrency market. This makes liquidity incentives an important part of a platform's features, to subsidize more staking and liquidity. It will depend on the volume of transactions, as the higher the volume is the greater the revenues collected. As more collateral is locked into the ecosystem's Vault, there is the potential of offsetting volatility with asset inflation and protocol fees. Asset inflation provides active participation that is rewarded for minting and staking tokens. Protocol fees generate the revenue that is paid back to liquidity providers for staking their tokens. These cancel out the amount of impermanent loss to further incentivize token holders.

 


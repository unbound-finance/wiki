# Unbound: A Derivative for AMMs



DeFi is evolving with various derivative layers and AMMs are building new smart contract based legos. Unbound is a DeFi platform that creates a treasury layer on top of existing AMM platforms by using LPT’s as a collateral, which is a decentralized receipt of the user’s funds in an AMM pool.    


Unbound provides the first-ever debt-free liquidity provision system! The platform provides liquidity to AMM LPTs and issues a Stablecoin \(UND\) in the form of a minted token. The platform unlocks the LPTs once the UND is returned, irrespective of time. The user is never at risk given that Unbound does not have a Liquidation Engine!  


![](https://lh5.googleusercontent.com/P8YOP6xSk5ONzXVEnfCXAKQ67GkMQ7lJoA902H1QJx7kH0TC4uoSvlH4JJoLgjq2aUhg1fnx1xxv6CIRbbcWa3BmUTONPHDLSz_qJ8ylE7vT79CLBYFlSu0gcYaqX42CG6-TZzUw)

1. Unlock LPT Liquidity: LPTs are the ideal collateral. They are great for funding but unsuitable for trading. Unbound will collateralize LPTs via smart contracts, which provide additional liquidity, without compromising on security.
2. Mint Stablecoin by locking LPTs: Unlock will lock LPTs and mint a stablecoin \(UND\).
3. No Liquidation Engine for LargeCap Pairs\(Eth/Dai,USDT/USDC,etc\) : Unbound does not have a liquidation engine. The smart contracts unlock collaterals whenever the minted UND is returned. What this imply is that when you mint UNDs, this does not create a debt position where:
   1. Users do not lose any collateral amount
   2. Unbound does not charge any penalty amount if the value of collateral goes below a certain amount.
4. SAFU fund: In case of an exceptionally steep decline in collateral value, the SAFU fund is there to absorb some or all of the losses without liquidating the user collateral. More details in the following sections.


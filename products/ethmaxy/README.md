---
description: A StETH 3x+ Yield earning token - For all ETH MaxY's pirates!
---

# 🔹 ETHMAXY

![](https://cdn-images-1.medium.com/max/800/0\*gBMWVxwJZ0i4-3k9)

The best leveraged $ETH liquid staking strategy in DeFi today, all within one tradable ERC20 token.

## ****:newspaper: **Fact Sheet**

### **Overview**

* Built on Set Protocol's battle-tested infrastructure, supporting the largest DeFi indices today.
* Utilises Lido for liquid staked Ethereum (stETH) and Aave to recursively leverage stETH and therefore its intrinsic yield properties.
* 1x ETH exposure, 3x+ leveraged stETH yield exposure, represented as a single ERC20 token.
* Tradable with deep liquidity on Uniswap V3.
* Minted with aSTETH (output ETHMAXY) using Set Protocol
* Redeemable with ETHMAXY & WETH (output aSTETH) using Set Protocol

### Methodology Parameters

**Target Leverage Ratio:** 3.25

**Minimum Leverage Ratio:** 3.00

**Max Leverage Ratio:** 3.30

**Rebalance Interval:** None, only when the leverage ratio moves out of the range parameters

### **Benefits**

* Offering outsized returns on ETH with low risk.
* The product remains as a fully composable token that can be utilised in DeFi.
* Abstracting the management of collateral and debt balances from the user.
* ETHMAXY Socializes gas costs associated with maintenance.
* Very low barrier to entry (a simple Uniswap trade).
* Highest staked, full composable ETH yield strategy token in the DeFi ecosystem.
* Yield is auto-compounding.

### **Risks**

Naturally, with leveraged positions, there is an inherent risk based on certain events occurring that are mitigated as much as possible by the product design. In the case of ETHMAXY, the risk of the product is liquidation in the event of a severe de-pegging of the stETH:ETH pairing. Specifically, if stETH reaches a 0.88/ETH ratio.

Our smart contract has the ability to adjust the leverage ratio in addition to a ripcord function to prevent liquidation risk in the face of negative conditions and is fully automated, therefore the product is marketed as very low risk when factoring in the sheer liquidity between stETH and ETH and the projected growth of both assets.

## :currency\_exchange: Where to Buy ETHMAXY:

You can buy the **ETH Max Yield Index** on Ethereum through:

* [**SetSwap** utilising 0x Routing](https://www.setswap.xyz/ethmaxy)
* [Uniswap V3 **ETHMAXY/WETH** pool.](https://app.uniswap.org/#/swap?inputCurrency=eth\&outputCurrency=0x0fe20e0fa9c78278702b05c333cc000034bb69e2\&chain=mainnet)

You can add liquidity on Sorbet Finance (Gelato):

* [Sorbet Finance (G-UNI pool).](https://www.sorbet.finance/#/pools/0x18D53f4953AD14236602DA05eFAfc0Df4f5d064D)&#x20;
* Want to earn rewards as an LP? [liquidity-rewards.md](liquidity-rewards.md "mention")&#x20;

## ****:ocean: **Diving Deeper - Leverage Tokens** <a href="#h_f547d7d43e" id="h_f547d7d43e"></a>

### **Summary** <a href="#h_f547d7d43e" id="h_f547d7d43e"></a>

Leverage tokens work by utilizing on-chain lending protocols, **** in ETHMAXYs case**,** Aave, by automatically adding/removing collateral to maintain a leverage position.

ETHMAXY aims to stay at a leverage ratio between 3 - 3.25x. This flexible rebalancing nature minimizes the number of rebalances, and thereby gas costs, to maintain a leveraged position.

### **Minting and Redeeming** <a href="#h_2e252564b6" id="h_2e252564b6"></a>

To understand how the leverage token works, first we will look at how it levers up and delevers.

The token starts off by supplying stETH as collateral to Aave to be able to borrow back WETH. In order to get the leverage, the protocol trades WETH for stETH using on-chain liquidity on a DEX like Uniswap. Finally, we put the stETH back into Aave and repeat the process to continue levering up the Set through **recursive lending and borrowing.**

Delivering works in a similar way, but in the opposite direction. recursively repaying back WETH debt and removing stETH collateral from Aave.

When somebody mints a new ETHMAXY token, the protocol takes their ETH and levers it to the current leverage ratio (between 3 - 3.30) using the mechanisms described above. When you mint, as opposed to buying the token directly from a DEX, you are going to get some WETH back along with the ETHMAXY token as that is part of the debt you are taking on.&#x20;

If you are buying directly from a DEX, don’t worry about this process, ETHMAXY has deep liquidity to facilitate the largest of orders.

### **Maintaining Leverage**

Naturally, as the value of stETH increases against ETH due to the intrinsic yield, the leverage ratio of ETHMAXY changes. In order to keep the leverage in line, a network of bots monitor the leverage condition and rebalance (using the levering and delivering processes described above) to take back the leverage ratio to a target of 3.25x.&#x20;

In the extreme case where the leverage ratio breaks out past the defined bounds of 3x - 3.30x, the protocol has a Ripcord function that engages in an emergency rebalance to bring it back within the bounds. \


## :notepad\_spiral: Contracts

* **G-UNI Pool:** [https://etherscan.io/address/0x18D53f4953AD14236602DA05eFAfc0Df4f5d064D](https://etherscan.io/address/0x18D53f4953AD14236602DA05eFAfc0Df4f5d064D)&#x20;
* **ETHMAXY:** [https://etherscan.io/token/0x0fe20e0fa9c78278702b05c333cc000034bb69e2](https://etherscan.io/token/0x0fe20e0fa9c78278702b05c333cc000034bb69e2)&#x20;
* **ETHMAXY BaseManager**: [https://etherscan.io/address/0xBc73791909e52119b5Cf47E8Bc22368141373Fce](https://etherscan.io/address/0xBc73791909e52119b5Cf47E8Bc22368141373Fce)&#x20;
* **FeeSplitExtension:** [https://etherscan.io/address/0x3782148481c75e16105A758134d0b5d939302518](https://etherscan.io/address/0x3782148481c75e16105A758134d0b5d939302518)
* **ETHMAXY Strategy:** [https://etherscan.io/address/0xB7439f887f0d61A236c8a14c22857684Dc5CD50e](https://etherscan.io/address/0xB7439f887f0d61A236c8a14c22857684Dc5CD50e)

## :books: Resources

* 📙 [Learn more about Galleon DAO](https://docs.galleon.community)
* [📘 Issuing and redeeming Sets using TokenSets](https://docs.tokensets.com/issue-and-redeem-sets)

***

For more information on **Galleon DAO**, please visit:

[Discord](https://discord.gg/galleondao) | [Twitter](https://twitter.com/GalleonDAO) | [Website](https://www.galleon.community)

For more information on **Beverage Finance**, please visit:

[Discord](https://discord.gg/pweUc3X6H4) | [Twitter](https://twitter.com/BeverageFinance) | [Website](https://beverage.finance)

\

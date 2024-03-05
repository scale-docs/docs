---

title: The EQUITY token
grand_parent:
parent: Equity
has_children:
nav_order: 3

---

# EQUITY: The Liquidity Token of Equity
> The Key to Unlock Boundless Earnings

Welcome to the realm of EQUITY token, the bedrock of our decentralized liquidity provision system. Delve into the flexibility of an index composed of various assets used for swaps. Seamlessly mint your EQUITY tokens with any index asset and redeem them into any index asset whenever you desire.

## Introduction
The EQUITY token is a "Share" representing the ownership of all the assets inside the Vault. It is essentially a Vault reciept denominated in eUSD, an internal, virtual index tracker that represents 1 USD. EQUITY can be freely minted or burned by adding or removing "Index Assets" of the Vault. 

## Price of EQUITY

### Formula
EQUITY token price for minting and redemption is calculated as:

```(Total value in eUSD of all assets in the vault)```

```divided by ```

```(Total Supply of EQUITY token)```

eUSD always represents 1 USD, and everything in the vault is denominated in it.

## Minting & Redeeming Equity
To mint EQUITY, a list of "Index Assets" can be found on our [Dashboard](https://equalizer.exchange).

Based on multiple on-chain price feeds and oracles, the price of all index assets is denominated in eUSD. While minting, an equivalent of 1 eUSD of any index-asset is used to mint 1 eUSD worth of EQUITY. Similarly, while redeeming 1 eUSD worth of EQUITY can be converted to any Index Assset worth 1 eUSD.

----
### Note:
#### There is a 15-minute cooldown period after minting new EQUITY. During this period it cannot be moved or staked or redeemed. This is an important security feature of the Protocol that protects it against blockchain & network outages.
----

## Rewards for owning EQUITY
As an EQUITY holder, you're entitled to a mix of EQUAL & veEQUAL (generally 70% veEQUAL & 30% EQUAL) proportional to the number of your staked EQUITY tokens. The amount of rewards and the Reward Rate is determined by the weekly vote and emission distribution on equalizer.exchange, the platform where weekly minted EQUAL is governed. All fees that are generated through the use of EQUITY liquidity are poured as Bribes to the Equalizer for lobbying a bigger EQUAL emission for the upcoming week.

## Market-making Fees
Each Mint & Redeem has an asscociated fees, charged as a small % of the EQUITY.

Minting fees are the opposite of Redeeming fees. An index asset with the lowest Minting Fee will have the highest Redeeming Fee, while the Index-Asset with the lowest Redemption Fee will have the maximum Mint Fee!

To make the most out of your investment, remember these points:
- Visit the "Fees" section to find tokens with the lowest fees.
- Use the token with the lowest fees to Mint or Redeem EQUITY pool.

## Rebalancing
The Market-making Fees mechanism encourages market-makers to rebalance the vault towards its desired Target Weights for all the involved Index Assets. Thus the lacking IAs will be encouraged to be added to the Vault, while the surplus assets will be encouraged to be redeemed.

Advanced traders with Smart contract skills can borrow tokens from Equalizer's CPAMM pools and arbitrage the discrepancy in fees on Equity vault to turn a profit.

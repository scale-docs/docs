---

title: Listing Special Tokens on Equalizer
nav_order: 7
has_children:
parent: List your Tokens

---

# List Special tokens

## Compatibility
Our Classic Volatile Pools fully support Trading and Liquidity additions of all Special tokens such as Rebasing tokens, Elastic Supply tokens, ERC404s, Fee-on-Transfer tokens, etc.

However, to earn the Trade Fees generated from such tokens, you must **exempt** the trade fees generated from double taxation.

Exotic tokens must make the `pairFees` address of all their pools exempt of any taxes or rebases, or else Liquidity Providers might not be able to claim the trade-fee rewards!

## Finding pair's "Fees" contract"
You can easily find it on the liquidity pool's ftmscan page on the 'Read Contract' tab under the **`fees`** heading.

## Effects of exemptions
Exempting the pair `Fees` address will not impact the transfer taxes taking place during trades or any other interactions with the liquidity pool. Your rebases or taxes will still work as expected. **This step only removes the taxes/rebases from the trade-fee portion, not the actual trade volume!**

## Gauges & Bribes
Equalizer's Gauges & Bribes are the First DEX to natively support Exotic tokens. **Gauges & Bribes Dont require special exemptions.**

But make sure to exempt the pair `Fees` address from any transfer-tax, rebase (positive or negative), Reflection rewards or other special features. If you dont, you wont be able to enjoy all the features of Equalizer!

## Correcting previously generated fees
In case you had not whitelisted the Fees address, it could have accrued a deficit of tokens. As in, if it ad expected 100 tokens and got only 99, it would think it has 100 but while transferring fees during fees claims, it would encounter an error and revert, since it has just 99 and not 100.

Solution to this is to simply sending it the remaining tokens.
- First of all, make sure it has been exempted or whitelisted by the Token's team or creator.
- Check how much of Fees was collected ever since the creation.
- Now transfer it the amount that might have been charged as a trade fees.
> If it was sent 500 tokens but received only 450 tokens (10% tax), then you need to send it the 50 tokens Plus some more to account for the taxation during your transfer to it. In this case, you should send it
> 50 (=10% of 500, the total lifetime fees)
> + 5 (=10% of 50, the deficit)
> + 1 (a little bit more)
> **= 56 tokens**
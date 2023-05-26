---

title: Trading with Equity
grand_parent:
parent: Equity
has_children:
nav_order: 4

---

# Embrace the Future of Trading with Equity!

Welcome to the exciting world of Equity, the state-of-the-art decentralized exchange that liberates you from the constraints of traditional trading. Forget usernames and passwords and dive right into the game! Our innovative aggregate price feed curbs the risk of liquidations from fleeting wicks, offering you a robust and reliable trading platform.

## Getting Started 

Are you new to the crypto universe? Fret not! We've got your back. If you're yet to get a wallet, we recommend using [Rabby](https://rabby.io/) or [MetaMask](https://metamask.io) for the best experience.

## Connecting Your Wallet 

Once your wallet is ready, it's time to connect it with our trading platform. It's as easy as clicking the "Connect Wallet" button on the Trade page. Should you encounter a message prompting you to "Add Fantom", go ahead and add the respective network to your wallet. Alternatively, you can manually add these networks for a more personalized experience. 

## Ensuring Uninterrupted Trading 

Being a decentralized exchange, Equity runs data queries and transactions through an RPC Server. Now, there might be times when the RPC lags, resulting in slow data load. During these periods, you can use an alternative or backup RPC to ensure uninterrupted trading. Just switch the RPC URL in the network settings of your wallet, and you're good to go! 

## Your First Steps in Trading 

To commence trading, you'll need to have FTM in your account. You can purchase FTM directly on Fantom using [Equalizer](https://equalizer.exchange/swap). Alternatively, you can transfer FTM to Fantom from other networks. Once the transfer is done, you're all set to embark on your trading journey. 

## Harness the Power of Swaps 

Equity proudly supports both swaps and leverage trading. For swaps, navigate to the "Swap" tab on our platform. Here, you can swap tokens effortlessly with zero price impact. To amplify your trading potential with leverage trading, follow the guidelines in the sections below. 

## Opening a Position 

To open a leverage position, you can select either "Long" or "Short." If you're betting on the token's price going up, opt for a long position. If you foresee the token's price going down, choose to open a Short. After selecting your side, enter the amount you wish to pay and the leverage you intend to use. 

## Position Management 

After initiating a trade, you can view it under your Positions list. Feel free to edit it as per your needs by depositing or withdrawing collateral. This allows you to efficiently manage your leverage and liquidation price. 

## Closing a Position 

Closing a position, be it partially or completely, is a breeze. Just hit the "Close" button and it's done! 

## Stop-Loss / Take-Profit Orders 

Want to hedge your risks and maximize your profits? Use our stop-loss and take-profit orders. Once a trigger order is set, it appears under the "Orders" tab. You can modify it anytime according to market conditions. 

## Partial Liquidations 

With Equity, you always have control over your positions. If the token's price crosses a certain point, your position will be automatically closed, ensuring you never lose more than you're willing to. 

## Pricing & Fees 

Equity offers competitive pricing with no price impacts for trades. Thus, you can execute large trades exactly at the mark price. Our fee structure is straightforward and transparent - just 0.1% of the position size to open/close a position. 

### Execution Fee

Opening, closing or modifying a position involves two distinct steps:

1. **Initiating the Transaction:** This is done by the user who sends the initial request to either open, close, adjust collateral, or withdraw from a position.

2. **Transaction Confirmation:** This is managed by 'Keepers' who monitor the blockchain for these requests and execute them.

The 'Execution Fee' represents the cost of the second step and is paid to the blockchain network. This fee is clearly displayed in the confirmation box prior to finalizing the transaction.

### Dealing with Stablecoin Price Fluctuations

In the event that a stablecoin's value diverges from the standard 1 USD:

**Short Positions:** Opening and concluding short positions in such circumstances could lead to an effect on the collateral, tied to a spread between the standard 1 USD and the current Chainlink rate of the stablecoin. For instance, should the stablecoin's value drop to 0.95 USD, initiating a position with 1000 units of the stablecoin would result in a collateral worth 950 USD, considering the 0.95 USD rate. On closing the position, 950 units of the stablecoin, evaluated at 1 USD rate, would be retracted. This method serves to prevent potential 'front-running' issues during price divergence, as collateral is stored in USD value and converted to tokens based on the latest rate.

**Short Position Profits:** Our contracts are designed to ensure complete profit payout for all short positions. Profit is disbursed in the stablecoin at the rate of 1 USD or the current Chainlink rate (whichever is higher).

**Swaps:** When swapping using a stablecoin with a diverged price, a similar spread to the Chainlink rate will be applied.

**Long Positions:** Long positions should remain largely unaffected. However, if there is a swap from a depegged stablecoin into the required collateral for a long position (for example, FTM), a spread may be observed. In such cases, alternative swap platforms can be utilized for the swap execution prior to initiating the long position. If a significant spread is detected, the user interface will provide a warning.


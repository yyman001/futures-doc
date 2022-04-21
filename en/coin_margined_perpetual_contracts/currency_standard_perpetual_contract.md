# Currency Standard Perpetual Contract

------

**Margin**

Unlike a USDT contract with USDT as a margin, a currency-based perpetual contract is a secured asset in the underlying currency, and the user needs to hold the corresponding currency to participate in the trading of the currency contract, such as a BTC/USD currency-based perpetual contract, and the user needs to transfer to BTC as a secured asset.

Because of the different currencies in which the guaranteed assets are used, the risk of depreciation of the guaranteed assets in both contracts varies when prices fall. Suppose that when the price of the BTC/USD currency is perpetual, the higher the requirement for the secured asset required for the user's position, the more BTC is required to hold the secured asset, but the USDT standard perpetual contract does not affect the value of the USDT secured asset because the required secured asset is USDT.

**Valuation Unit**

A USDT standard perpetual contract is denominated in USDT and a currency standard perpetual contract is denominated in US dollars. "Thus the index prices between the two will also vary, e.g. the BTC/USDT index price is the price taken from the BTC spot to USDT on each exchange, and the BTC/USD currency standard perpetual contract is the price taken from the BTC spot USD on each exchange."

**The face value of the contract**

The value of each contract for USDT standard per contract is the corresponding underlying currency, e.g. BTC/USDT has a face value of 0.001BTC, and the value of each contract is USD, e.g. BTC/USD is $100.

**Profit and loss currency**

All type of contracts of the USDT standard perpetual contract use the denominated currency USDT to calculate profit or loss, and the currency standard perpetual contract calculates the profit or loss in the underlying currency, e.g. the user trades the BTC/USD currency standard perpetual contract in the currency BTC.
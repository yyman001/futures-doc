# Margin and profit/loss calculations

------

**Open position margin**

Open position margin is the minimum collateral amount required to open a position in a leveraged trade. The leverage multiple used by the trader is inversely proportional to the opening margin required to open a position. The higher the leverage, the less margin is required to open a position.

In a USDT perpetual contract, the opening margin is obtained by multiplying the principal value by the initial margin rate. The starting margin rate depends on the multiple of leverage used.

Open position margin= Contract quantity * entry price/leverage

***Example:***

Traders use 50x leverage to open a 1 BTC long order at $10,000.
Starting margin= (1 x 10,000)/ 50= 200 USDT

**Average opening price**

When an open position occurs, the average price of the open position is recalculated.

Example: Trader A now holds multiple positions of BTCUSDT long position 0.5, opening price of 5000 USD. An hour later, Trader A decides to open an additional 0.3 position at 6,000 USD.

Below are the formulas and calculation steps for the average opening average price:

* Average open price= USDT total contract value/total contract quantity
* Total contract value in USDT= [ (contract quantity 1 * price 1) + (contract quantity 2 * price 2)...]

We obtain the following data:

The total value of the contract in USDT

=[(Contract quantity 1 x price 1) + ( contract quantity 2 x price 2)]
= [ (0.5 x 5000) + (0.3 x 6000) ]
= 4300

Contract total quantity

= 0.5 + 0.3
= 0.8 BTC

Average opening price

= 4300 / 0.8
= 5375

**Profit/loss**

After opening a position, the position and its profit and loss can be seen in real time in the position area.

Depending on the direction of your trade, the formula for calculating profit and loss is slightly different.
For multiple positions

***Example:***

Trader B now holds multiple positions of BTCUSDT long position 0.2, opening price of 7000 USDT. When the latest market price in the order table is shown as 7,500 USD, the unresolved profit and loss is displayed as 100 USDT.

```
Profit/loss= Contract quantity x (marked price - average opening price)
```

= 0.2 x (7500 - 7000)

= 100 USDT

For short positions

***Example:***

Trader C now holds a short position of BTCUSDT short position 0.4, opening price of 6000 USD. When the latest market price in the order table is shown as 5,000 USD, the unresolved profit and loss is displayed as 400 USDT.

```
Profit/loss= Contract quantity x (average opening price - marked price)
```
= 0.4 x (6000 - 5000)
= 400 USDT
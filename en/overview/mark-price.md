# Mark Price

**What is a marked price?**

In order to improve the stability of the contract market and reduce unnecessary forced closing when the market is abnormally volatile, we use the marked price to calculate the user's unrealized profit and loss and trigger a forced reduction.

**Marked price algorithm**

Marked Price= Median number (latest price, reasonable price, moving average price)

Meaning the following:

```
Latest Price= The Exchange's Median Price (Buy 1, Sell 1, Trade Price)

Reasonable price= index price * (1 + capital rate of the previous period * (time between now and the next charge of funds / the interval between the collection of funds rate)

Moving Average Price= Index Price + 60 - Minute Moving Average (Spread)
Spreads= The exchange's median price - index price
```

The marked price takes into account both the spot index price and the moving average of the base deviation. The moving average mechanism smoothly filters contract price fluctuations over a short period of time, reducing unnecessary forced closings due to abnormal fluctuations.
# Index Price
>What is index price?

The index price is based on the latest transaction price of the standard currency pair of the mainstream exchange in the market and the median buy-to-sell median, weighted average, calculated and obtained index price, which can represent the fair market price of the currency pair.

The following are the source exchanges and calculated weights for each contract index.

USDT contract

| Contract | FTX | Huobi | Binance |
| :------: | :-: | :---: | :-----: |
| BTCUSDT  | 1%  |  1%   |   1%    |
| ETHUSDT  | 1%  |  1%   |   1%    |
| ETCUSDT  | ~~  |  1%   |   1%    |
| DOGEUSDT | ~~  |  ~~   |   20%   |
| LTCUSDT  | 1%  |  1%   |   1%    |
| ADAUSDT  | ~~  |  1%   |   1%    |
| TRXUSDT  | 1%  |  1%   |   1%    |
| BCHUSDT  | 1%  |  1%   |   1%    |
| SOLUSDT  | ~~  |  ~~   |   20%   |
| XLMUSDT  | ~~  |  ~~   |   20%   |

Standard currency Contract

| Contract | FTX | Coinbase | Bitfinex |
| :------: | :-: | :------: | :------: |
|  BTCUSD  | 1%  |    1%    |    1%    |
|  ETHUSD  | 1%  |    1%    |    1%    |
|  LTCUSD  | 20% |   20%    |    ~~    |

[The above data and indicator content may be adjusted in real time according to market conditions, the adjustment will not be notified.]

Sample data sampling: Gets the latest prices for exchanges in the table through the API every 1 second, depending on the interval at which the index is updated.

**Index exception handling**

- Removing invalid prices:

When any source exchange price is not updated within 40000ms and the value of the previous value is too different, we will assume that its price is mistaken, at this calculation the right to reset the exchange to 0.

- Abnormal price correction:

When the price of an exchange deviates significantly from that of other exchanges and the median deviation of the price of all source exchanges (including the exchange itself) by ±3%, the price of that exchange is calculated at the median ±3% of the sample exchange price (when the median deviation of the USDT price reaches ±0.3%, the price of that exchange is calculated at the median ±0.3% of the sample exchange price).

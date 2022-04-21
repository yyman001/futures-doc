# Leverage and position limit

---

Risk limits are a risk management mechanism used to limit a trader's position risk. In a volatile trading environment, a single trader holding a large position with high leverage can result in significant losses. The system uses the concept of dynamic leverage, i.e. the maximum leverage available for trading will vary depending on the value of the position held by the trader: the greater the value of the position held, the lower the maximum leverage available. At the same time, the larger the leverage selected, the smaller the open position.

**BTCUSD Contract**

| Position nominal value（BTC） | Maximum leverage |
| :---------------------------- | :--------------- |
| 0 ~ 5                         | 125x             |
| 5 ~ 10                        | 100x             |
| 10 ~ 20                       | 50x              |
| 20 ~ 50                       | 20x              |
| 50 ~ 100                      | 10x              |
| 100 ~ 200                     | 5x               |
| 200 ~ 400                     | 4x               |
| 400 ~ 1000                    | 3x               |
| 1000 ~ 1500                   | 2x               |
| 1500 ~ 2500                   | 1x               |

**ETHUSD Contract**

| Position nominal value（ETH） | Maximum leverage |
| :---------------------------- | :--------------- |
| 0 ~15                         | 100x             |
| 15 ~100                       | 75x              |
| 100 ~250                      | 50x              |
| 250 ~500                      | 20x              |
| 500 ~1,000                    | 10x              |
| 1,000 ~1,500                  | 5x               |
| 1,500 ~2,000                  | 4x               |
| 2,000 ~5,000                  | 3x               |
| 5,000 ~7,500                  | 2x               |
| 7,500 ~50,000                 | 1x               |

**LTCUSD Contract**
| Position nominal value（LTC） | Maximum leverage |
| :---------------------------- | :--------------- |
| 0 ~2,500                      | 20x              |
| 2,500 ~5,000                  | 10x              |
| 5,000 ~10,000                 | 7x               |
| 10,000 ~25,000                | 6x               |
| 25,000 ~50,000                | 5x               |
| 50,000 ~75,000                | 4x               |
| 75,000 ~100,000               | 3x               |
| 100,000 ~125,000              | 2x               |
| \> 125,000                    | 1x               |

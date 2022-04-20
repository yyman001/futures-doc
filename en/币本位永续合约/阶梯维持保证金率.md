# Ladder Maintenance Margin Rate

---

**Maintenance margin rate**

Margin rate is a measure of the risk of position-guaranteed assets, maintenance margin is the minimum margin rate of a position, when the position margin rate reaches the maintenance margin rate, your position will be forced to be taken over by the system. We use the marked price to calculate margin rates to avoid forced closing due to non-liquidity or market manipulation.

**Ladder maintenance margin rates**

In order to prevent large positions from bursting from the impact on market liquidity, resulting in large losses, we use a ladder mechanism to reduce positions. Each ladder corresponds to a different maintenance margin rate, when the system determines that the margin is not enough for the current position of the position of the maintenance margin, it will carry out the operation of reducing the number of positions to the next position in the ladder.

**BTCUSD Contract**

| Position nominal value（BTC） | Maintenance margin rate |
| :---------------------------- | :---------------------- |
| 0 ~ 5                         | 0.40%                   |
| 5~10                          | 0.50%                   |
| 10 ~ 20                       | 1%                      |
| 20 ~ 50                       | 2.50%                   |
| 50 ~ 100                      | 5%                      |
| 100 ~ 200                     | 10%                     |
| 200 ~ 400                     | 12.50%                  |
| 400 ~ 1,000                   | 15%                     |
| 1,000 ~ 1,500                 | 25%                     |
| 1,500 ~ 2,500                 | 50%                     |

**ETHUSD Contract**

| Position nominal value（ETH） | Maintenance margin rate |
| :---------------------------- | :---------------------- |
| 0 ~ 15                        | 0.5%                    |
| 15 ~ 100                      | 0.65%                   |
| 100 ~ 250                     | 1%                      |
| 250 ~ 500                     | 2.5%                    |
| 500 ~ 1,000                   | 5%                      |
| 1,000 ~ 1,500                 | 10%                     |
| 1,500 ~ 2,000                 | 12.5%                   |
| 2,000 ~ 5,000                 | 15%                     |
| 5,000 ~ 7,500                 | 25%                     |
| 7,500 ~ 50,000                | 50%                     |

**LTCUSD Contract**

| Position nominal value（ETH） | Maintenance margin rate |
| :---------------------------- | :---------------------- |
| 0 ~ 2,500                     | 2.5%                    |
| 2,500 ~ 5,000                 | 5%                      |
| 5,000 ~ 10,000                | 5%                      |
| 10,000 ~ 25,000               | 5%                      |
| 25,000 ~ 50,000               | 10%                     |
| 50,000 ~ 75,000               | 12.5%                   |
| 75,000 ~ 100,000              | 15%                     |
| 100,000 ~ 125,000             | 25%                     |
| 125,000 ~ 10,000,000          | 50%                     |

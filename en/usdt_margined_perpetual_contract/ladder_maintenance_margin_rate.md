# Ladder Maintenance Margin Rate

**Maintenance margin rate**

Margin rate is a measure of the risk of position-guaranteed assets, maintenance margin is the minimum margin rate of a position, when the position margin rate reaches the maintenance margin rate, your position will be forced to be taken over by the system. We use the marked price to calculate margin rates to avoid forced closing due to non-liquidity or market manipulation.

**Ladder maintenance margin rates**

In order to prevent large positions from bursting from the impact on market liquidity, resulting in large losses, we use a ladder mechanism to reduce positions. Each ladder corresponds to a different maintenance margin rate, when the system determines that the margin is not enough for the current position of the position of the maintenance margin, it will carry out the operation of reducing the number of positions to the next position in the ladder.


**BTCUSDT Contract**

| Position nominal value (USDT) | Maintenance Margin Rate |
| ----------------------------- | ----------------------- |
| 0~50,000                      | 0.40%                   |
| 50,000~250,000                | 0.50%                   |
| 250,000~1,000,000             | 1.00%                   |
| 1,000,000~7,500,000           | 2.50%                   |
| 7,500,000~40,000,000          | 5.00%                   |
| 40,000,000~100,000,000        | 10.00%                  |
| 100,000,000~200,000,000       | 12.50%                  |
| 200,000,000~400,000,000       | 15.00%                  |
| 400,000,000~600,000.000       | 25.00%                  |
| 600,000,000~1,000,000.000     | 50.00%                  |

**ETHUSDT Contract**

| Position nominal value (USDT) | Maintenance Margin Rate |
| ----------------------------- | ----------------------- |
| 0~10,000                      | 0.50%                   |
| 10,000~100,000                | 0.65%                   |
| 100,000~500,000               | 1.00%                   |
| 500,000~1,500,000             | 2.00%                   |
| 1,500,000~4,000,000           | 5.00%                   |
| 4,000,000~10,000,000          | 10.00%                  |
| 10,000,000~20,000,000         | 12.50%                  |
| 20,000,000~40,000,000         | 15.00%                  |
| 40,000,000~150,000,000        | 25.00%                  |
| 150,000,000~500,000,000       | 50.00%                  |

**LTCUSDT Contract**

| Position nominal value (USDT) | Maintenance Margin Rate |
| ----------------------------- | ----------------------- |
| 0~10,000                      | 0.65%                   |
| 10,000~50,000                 | 1.00%                   |
| 50,000~250,000                | 2.00%                   |
| 250,000~1,000,000             | 5.00%                   |
| 1,000,000~2,000,000           | 10.00%                  |
| 2,000,000~5,000,000           | 12.50%                  |
| 5,000,000~10,000,000          | 15.00%                  |
| 10,000,000~20,000,000         | 25.00%                  |
| 20,000,000~50,000,000         | 50.00%                  |

**ETCUSDT Contract**

| Position nominal value (USDT) | Maintenance Margin Rate |
| ----------------------------- | ----------------------- |
| 0~10,000                      | 0.65%                   |
| 10,000~50,000                 | 1.00%                   |
| 50,000~250,000                | 2.00%                   |
| 250,000~1,000,000             | 5.00%                   |
| 1,000,000~2,000,000           | 10.00%                  |
| 2,000,000~5,000,000           | 12.50%                  |
| 5,000,000~10,000,000          | 15.00%                  |
| 10,000,000~20,000,000         | 25.00%                  |
| 20,000,000~50,000,000         | 50.00%                  |

**DOGEUSDT Contract**

| Position nominal value (USDT) | Maintenance Margin Rate |
| ----------------------------- | ----------------------- |
| 0~50,000                      | 1.00%                   |
| 50,000~250,000                | 2.50%                   |
| 250,000~1,000,000             | 5.00%                   |
| 1,000,000~2,000,000           | 10.00%                  |
| 2,000,000~5,000,000           | 12.50%                  |
| 5,000,000~10,000,000          | 25.00%                  |
| 10,000,000~50,000,000         | 50.00%                  |

**ADAUSDT Contract**

| Position nominal value (USDT) | Maintenance Margin Rate |
| ----------------------------- | ----------------------- |
| 0~10,000                      | 0.65%                   |
| 10,000~50,000                 | 1.00%                   |
| 50,000~250,000                | 2.00%                   |
| 250,000~1,000,000             | 5.00%                   |
| 1,000,000~2,000,000           | 10.00%                  |
| 2,000,000~5,000,000           | 12.50%                  |
| 5,000,000~10,000,000          | 15.00%                  |
| 10,000,000~20,000,000         | 25.00%                  |
| 20,000,000~50,000,000         | 50.00%                  |

**TRXUSDT Contract**

| Position nominal value (USDT) | Maintenance Margin Rate |
| ----------------------------- | ----------------------- |
| 0~10,000                      | 0.65%                   |
| 10,000~50,000                 | 1.00%                   |
| 50,000~250,000                | 2.00%                   |
| 250,000~1,000,000             | 5.00%                   |
| 1,000,000~2,000,000           | 10.00%                  |
| 2,000,000~5,000,000           | 12.50%                  |
| 5,000,000~10,000,000          | 15.00%                  |
| 10,000,000~20,000,000         | 25.00%                  |
| 20,000,000~50,000,000         | 50.00%                  |

**BCHUSDT Contract**

| Position nominal value (USDT) | Maintenance Margin Rate |
| ----------------------------- | ----------------------- |
| 0~10,000                      | 0.65%                   |
| 10,000~50,000                 | 1.00%                   |
| 50,000~250,000                | 2.00%                   |
| 250,000~1,000,000             | 5.00%                   |
| 1,000,000~2,000,000           | 10.00%                  |
| 2,000,000~5,000,000           | 12.50%                  |
| 5,000,000~10,000,000          | 15.00%                  |
| 10,000,000~20,000,000         | 25.00%                  |
| 20,000,000~50,000,000         | 50.00%                  |

**SOLUSDT Contract**

| Position nominal value (USDT) | Maintenance Margin Rate |
| ----------------------------- | ----------------------- |
| 0~50,000                      | 1.00%                   |
| 50,000~250,000                | 2.50%                   |
| 250,000~1,000,000             | 5.00%                   |
| 1,000,000~2,000,000           | 10.00%                  |
| 2,000,000~5,000,000           | 12.50%                  |
| 5,000,000~10,000,000          | 25.00%                  |
| 10,000,000~50,000,000         | 50.00%                  |

**XLMUSDT Contract**

| Position nominal value (USDT) | Maintenance Margin Rate |
| ----------------------------- | ----------------------- |
| 0~10,000                      | 0.65%                   |
| 10,000~50,000                 | 1.00%                   |
| 50,000~250,000                | 2.00%                   |
| 250,000~1,000,000             | 5.00%                   |
| 1,000,000~2,000,000           | 10.00%                  |
| 2,000,000~5,000,000           | 12.50%                  |
| 5,000,000~10,000,000          | 15.00%                  |
| 10,000,000~20,000,000         | 25.00%                  |
| 20,000,000~50,000,000         | 50.00%                  |

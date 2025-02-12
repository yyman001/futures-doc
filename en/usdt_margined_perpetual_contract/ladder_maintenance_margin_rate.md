# Ladder Maintenance Margin Rate

**Maintenance margin rate**

Margin rate is a measure of the risk of position-guaranteed assets, maintenance margin is the minimum margin rate of a position, when the position margin rate reaches the maintenance margin rate, your position will be forced to be taken over by the system. We use the marked price to calculate margin rates to avoid forced closing due to non-liquidity or market manipulation.

**Ladder maintenance margin rates**

In order to prevent large positions from bursting from the impact on market liquidity, resulting in large losses, we use a ladder mechanism to reduce positions. Each ladder corresponds to a different maintenance margin rate, when the system determines that the margin is not enough for the current position of the position of the maintenance margin, it will carry out the operation of reducing the number of positions to the next position in the ladder.


**BTCUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0~50,000                      | 0.40%                   |
| 2     | 50,000~250,000                | 0.50%                   |
| 3     | 250,000~1,000,000             | 1.00%                   |
| 4     | 1,000,000~7,500,000           | 2.50%                   |
| 5     | 7,500,000~40,000,000          | 5.00%                   |
| 6     | 40,000,000~100,000,000        | 10.00%                  |
| 7     | 100,000,000~200,000,000       | 12.50%                  |
| 8     | 200,000,000~400,000,000       | 15.00%                  |
| 9     | 400,000,000~600,000.000       | 25.00%                  |
| 10    | 600,000,000~1,000,000.000     | 50.00%                  |

**ETHUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0~10,000                      | 0.50%                   |
| 2     | 10,000~100,000                | 0.65%                   |
| 3     | 100,000~500,000               | 1.00%                   |
| 4     | 500,000~1,500,000             | 2.00%                   |
| 5     | 1,500,000~4,000,000           | 5.00%                   |
| 6     | 4,000,000~10,000,000          | 10.00%                  |
| 7     | 10,000,000~20,000,000         | 12.50%                  |
| 8     | 20,000,000~40,000,000         | 15.00%                  |
| 9     | 40,000,000~150,000,000        | 25.00%                  |
| 10    | 150,000,000~500,000,000       | 50.00%                  |

**LTCUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0~10,000                      | 0.65%                   |
| 2     | 10,000~50,000                 | 1.00%                   |
| 3     | 50,000~250,000                | 2.00%                   |
| 4     | 250,000~1,000,000             | 5.00%                   |
| 5     | 1,000,000~2,000,000           | 10.00%                  |
| 6     | 2,000,000~5,000,000           | 12.50%                  |
| 7     | 5,000,000~10,000,000          | 15.00%                  |
| 8     | 10,000,000~20,000,000         | 25.00%                  |
| 9     | 20,000,000~50,000,000         | 50.00%                  |

**ETCUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0~10,000                      | 0.65%                   |
| 2     | 10,000~50,000                 | 1.00%                   |
| 3     | 50,000~250,000                | 2.00%                   |
| 4     | 250,000~1,000,000             | 5.00%                   |
| 5     | 1,000,000~2,000,000           | 10.00%                  |
| 6     | 2,000,000~5,000,000           | 12.50%                  |
| 7     | 5,000,000~10,000,000          | 15.00%                  |
| 8     | 10,000,000~20,000,000         | 25.00%                  |
| 9     | 20,000,000~50,000,000         | 50.00%                  |

**DOGEUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0~50,000                      | 1.00%                   |
| 2     | 50,000~250,000                | 2.50%                   |
| 3     | 250,000~1,000,000             | 5.00%                   |
| 4     | 1,000,000~2,000,000           | 10.00%                  |
| 5     | 2,000,000~5,000,000           | 12.50%                  |
| 6     | 5,000,000~10,000,000          | 25.00%                  |
| 7     | 10,000,000~50,000,000         | 50.00%                  |

**ADAUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0~10,000                      | 0.65%                   |
| 2     | 10,000~50,000                 | 1.00%                   |
| 3     | 50,000~250,000                | 2.00%                   |
| 4     | 250,000~1,000,000             | 5.00%                   |
| 5     | 1,000,000~2,000,000           | 10.00%                  |
| 6     | 2,000,000~5,000,000           | 12.50%                  |
| 7     | 5,000,000~10,000,000          | 15.00%                  |
| 8     | 10,000,000~20,000,000         | 25.00%                  |
| 9     | 20,000,000~50,000,000         | 50.00%                  |

**TRXUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0~10,000                      | 0.65%                   |
| 2     | 10,000~50,000                 | 1.00%                   |
| 3     | 50,000~250,000                | 2.00%                   |
| 4     | 250,000~1,000,000             | 5.00%                   |
| 5     | 1,000,000~2,000,000           | 10.00%                  |
| 6     | 2,000,000~5,000,000           | 12.50%                  |
| 7     | 5,000,000~10,000,000          | 15.00%                  |
| 8     | 10,000,000~20,000,000         | 25.00%                  |
| 9     | 20,000,000~50,000,000         | 50.00%                  |

**BCHUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0~10,000                      | 0.65%                   |
| 2     | 10,000~50,000                 | 1.00%                   |
| 3     | 50,000~250,000                | 2.00%                   |
| 4     | 250,000~1,000,000             | 5.00%                   |
| 5     | 1,000,000~2,000,000           | 10.00%                  |
| 6     | 2,000,000~5,000,000           | 12.50%                  |
| 7     | 5,000,000~10,000,000          | 15.00%                  |
| 8     | 10,000,000~20,000,000         | 25.00%                  |
| 9     | 20,000,000~50,000,000         | 50.00%                  |

**SOLUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0~50,000                      | 1.00%                   |
| 2     | 50,000~250,000                | 2.50%                   |
| 3     | 250,000~1,000,000             | 5.00%                   |
| 4     | 1,000,000~2,000,000           | 10.00%                  |
| 5     | 2,000,000~5,000,000           | 12.50%                  |
| 6     | 5,000,000~10,000,000          | 25.00%                  |
| 7     | 10,000,000~50,000,000         | 50.00%                  |

**XLMUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0~10,000                      | 0.65%                   |
| 2     | 10,000~50,000                 | 1.00%                   |
| 3     | 50,000~250,000                | 2.00%                   |
| 4     | 250,000~1,000,000             | 5.00%                   |
| 5     | 1,000,000~2,000,000           | 10.00%                  |
| 6     | 2,000,000~5,000,000           | 12.50%                  |
| 7     | 5,000,000~10,000,000          | 15.00%                  |
| 8     | 10,000,000~20,000,000         | 25.00%                  |
| 9     | 20,000,000~50,000,000         | 50.00%                  |

**APTUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0 - 50,000                    | 1.00%                   |
| 2     | 50,000 - 250,000              | 2.50%                   |
| 3     | 250,000 - 1,000,000           | 5.00%                   |
| 4     | 1,000,000 - 2,000,000         | 10.00%                  |
| 5     | 2,000,000 - 5,000,000         | 12.50%                  |
| 6     | 5,000,000 - 10,000,000        | 25.00%                  |
| 7     | 10,000,000 - 20,000,000       | 50.00%                  |

**FILUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0 - 50,000                    | 1.00%                   |
| 2     | 50,000 - 250,000              | 2.00%                   |
| 3     | 250,000 - 1,000,000           | 5.00%                   |
| 4     | 1,000,000 - 2,000,000         | 10.00%                  |
| 5     | 2,000,000 - 5,000,000         | 12.50%                  |
| 6     | 5,000,000 - 10,000,000        | 16.65%                  |
| 7     | 10,000,000 - 20,000,000       | 25.00%                  |
| 8     | 20,000,000 - 30,000,000       | 50.00%                  |


**AAVEUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0 - 5,000                     | 1.00%                   |
| 2     | 5,000 - 25,000                | 2.50%                   |
| 3     | 25,000 - 100,000              | 5.00%                   |
| 4     | 100,000 - 250,000             | 10.00%                  |
| 5     | 250,000 - 1,000,000           | 12.50%                  |
| 6     | 1,000,000 - 5,000,000         | 50.00%                  |

**LINKUSDT Contract**

| Level | Position nominal value (USDT) | Maintenance Margin Rate |
| ----- | ----------------------------- | ----------------------- |
| 1     | 0 - 10000                     | 0.65%                   |
| 2     | 10,000 - 50,000               | 1.00%                   |
| 3     | 50,000 - 250,000              | 2.00%                   |
| 4     | 250,000 - 1000,000            | 5.00%                   |
| 5     | 1,000,000 - 2,000,000         | 10.00%                  |
| 6     | 2,000,000 - 5,000,000         | 12.50%                  |
| 7     | 5,000,000 - 10,000,000        | 15.00%                  |
| 8     | 10,000,000 - 20,000,000       | 25.00%                  |
| 9     | 20,000,000 - 50,000,000       | 50.00%                  |

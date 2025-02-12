# 杠杆和持仓上限


风险限额是用于限制交易者持仓风险的一种风险管理机制。在价格波动大的交易环境下，单一使用高杠杆持有大额仓位的交易者将可能带来巨大的穿仓损失。本系统使用动态杠杆的概念，即交易时可以使用的最大杠杆将根据交易者所持有的仓位价值而改变：持有的仓位价值越大，可使用的最大杠杆也越低。同时，选择越大的杠杆，可开的仓位也就越小。

**BTCUSDT 合约**

| 杠杆      | 最大可持仓名义价值（USDT） |
| --------- | -------------------------- |
| 0x~1x     | 1,000,000,000              |
| 1x~2x     | 600,000,000                |
| 2x~3x     | 400,000,000                |
| 3x~4x     | 200,000,000                |
| 4x~5x     | 100,000,000                |
| 5x~10x    | 40,000,000                 |
| 10x~20x   | 7,500,000                  |
| 20x~50x   | 1,000,000                  |
| 50x~100x  | 250,000                    |
| 100x~125x | 50,000                     |

**ETHUSDT 合约**

| 杠杆     | 最大可持仓名义价值（USDT） |
| -------- | -------------------------- |
| 0x~1x    | 500,000,000                |
| 1x~2x    | 150,000,000                |
| 2x~3x    | 40,000,000                 |
| 3x~4x    | 20,000,000                 |
| 4x~5x    | 10,000,000                 |
| 5x~10x   | 4,000,000                  |
| 10x~25x  | 1,500,000                  |
| 25x~50x  | 500,000                    |
| 50x~75x  | 100,000                    |
| 75x~100x | 10,000                     |

**LTCUSDT 合约**

| 杠杆    | 最大可持仓名义价值（USDT） |
| ------- | -------------------------- |
| 0x~1x   | 50,000,000                 |
| 1x~2x   | 20,000,000                 |
| 2x~3x   | 10,000,000                 |
| 3x~4x   | 5,000,000                  |
| 4x~5x   | 2,000,000                  |
| 5x~10x  | 1,000,000                  |
| 10x~25x | 250,000                    |
| 25x~50x | 50,000                     |
| 50x~75x | 10,000                     |

**ETCUSDT 合约**

| 杠杆    | 最大可持仓名义价值（USDT） |
| ------- | -------------------------- |
| 0x~1x   | 50,000,000                 |
| 1x~2x   | 20,000,000                 |
| 2x~3x   | 10,000,000                 |
| 3x~4x   | 5,000,000                  |
| 4x~5x   | 2,000,000                  |
| 5x~10x  | 1,000,000                  |
| 10x~25x | 250,000                    |
| 25x~50x | 50,000                     |
| 50x~75x | 10,000                     |

**DOGEUSDT 合约**

| 杠杆    | 最大可持仓名义价值（USDT） |
| ------- | -------------------------- |
| 0x~1x   | 50,000,000                 |
| 1x~2x   | 10,000,000                 |
| 2x~4x   | 5,000,000                  |
| 4x~5x   | 2,000,000                  |
| 5x~10x  | 1,000,000                  |
| 10x~20x | 250,000                    |
| 20x~50x | 50,000                     |

**ADAUSDT 合约**

| 杠杆    | 最大可持仓名义价值（USDT） |
| ------- | -------------------------- |
| 0x~1x   | 50,000,000                 |
| 1x~2x   | 20,000,000                 |
| 2x~3x   | 10,000,000                 |
| 3x~4x   | 5,000,000                  |
| 4x~5x   | 2,000,000                  |
| 5x~10x  | 1,000,000                  |
| 10x~25x | 250,000                    |
| 25x~50x | 50,000                     |
| 50x~75x | 10,000                     |

**TRXUSDT 合约**

| 杠杆    | 最大可持仓名义价值（USDT） |
| ------- | -------------------------- |
| 0x~1x   | 50,000,000                 |
| 1x~2x   | 20,000,000                 |
| 2x~3x   | 10,000,000                 |
| 3x~4x   | 5,000,000                  |
| 4x~5x   | 2,000,000                  |
| 5x~10x  | 1,000,000                  |
| 10x~25x | 250,000                    |
| 25x~50x | 50,000                     |
| 50x~75x | 10,000                     |

**BCHUSDT 合约**

| 杠杆    | 最大可持仓名义价值（USDT） |
| ------- | -------------------------- |
| 0x~1x   | 50,000,000                 |
| 1x~2x   | 20,000,000                 |
| 2x~3x   | 10,000,000                 |
| 3x~4x   | 5,000,000                  |
| 4x~5x   | 2,000,000                  |
| 5x~10x  | 1,000,000                  |
| 10x~25x | 250,000                    |
| 25x~50x | 50,000                     |
| 50x~75x | 10,000                     |

**SOLUSDT 合约**

| 杠杆    | 最大可持仓名义价值（USDT） |
| ------- | -------------------------- |
| 0x~1x   | 50,000,000                 |
| 1x~2x   | 10,000,000                 |
| 2x~4x   | 5,000,000                  |
| 4x~5x   | 2,000,000                  |
| 5x~10x  | 1,000,000                  |
| 10x~20x | 250,000                    |
| 20x~50x | 50,000                     |

**XLMUSDT 合约**

| 杠杆    | 最大可持仓名义价值（USDT） |
| ------- | -------------------------- |
| 0x~1x   | 50,000,000                 |
| 1x~2x   | 20,000,000                 |
| 2x~3x   | 10,000,000                 |
| 3x~4x   | 5,000,000                  |
| 4x~5x   | 2,000,000                  |
| 5x~10x  | 1,000,000                  |
| 10x~25x | 250,000                    |
| 25x~50x | 50,000                     |
| 50x~75x | 10,000                     |


**APTUSDT 合约**

| 杠杆      | 最大可持仓名义价值（USDT） |
| --------- | -------------------------- |
| 0x ~ 1x   | 20,000,000                 |
| 1x ~ 2x   | 10,000,000                 |
| 2x ~ 4x   | 5,000,000                  |
| 4x ~ 5x   | 2,000,000                  |
| 5x ~ 10x  | 1,000,000                  |
| 10x ~ 20x | 250,000                    |
| 20x ~ 50x | 50,000                     |

**FILUSDT 合约**

| 杠杆      | 最大可持仓名义价值（USDT） |
| --------- | -------------------------- |
| 0x ~ 1x   | 30,000,000                 |
| 1x ~ 2x   | 20,000,000                 |
| 2x ~ 3x   | 10,000,000                 |
| 3x ~ 4x   | 5,000,000                  |
| 4x ~ 5x   | 2,000,000                  |
| 5x ~ 10x  | 1,000,000                  |
| 10x ~ 25x | 250,000                    |
| 25x ~ 50x | 50,000                     |

**AAVEUSDT 合约**

| 杠杆      | 最大可持仓名义价值（USDT） |
| --------- | -------------------------- |
| 0x ~ 1x   | 5,000,000                  |
| 1x ~ 2x   | 1,000,000                  |
| 2x ~ 5x   | 250,000                    |
| 5x ~ 10x  | 100,000                    |
| 10x ~ 20x | 25,000                     |
| 20x ~ 25x | 5,000                      |

**LINKUSDT 合约**

| 杠杆      | 最大可持仓名义价值（USDT） |
| --------- | -------------------------- |
| 0x ~ 1x   | 50,000,000                 |
| 1x ~ 2x   | 20,000,000                 |
| 2x ~ 3x   | 10,000,000                 |
| 3x ~ 4x   | 5,000,000                  |
| 4x ~ 5x   | 2,000,000                  |
| 5x ~ 10x  | 1,000,000                  |
| 10x ~ 25x | 250,000                    |
| 25x ~ 50x | 50,000                     |
| 50x ~ 75x | 10,000                     |

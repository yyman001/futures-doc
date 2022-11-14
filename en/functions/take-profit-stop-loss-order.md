# Take Profit Stop Loss Order

**Pre-knowledge: position stop profit and loss**

Set stop loss on [position - stop profit] !

[Stop profit and loss on position](take_profit_stop_loss_tp_sl.md##如何设置止盈止损)

## What is a take profit stop loss order (preset Take Profit stop loss)?

When there is a position, you can set TP/SL at the [Position -Take Profit Stop Loss], but when there is only one open order and the position has not yet been formed, how can we set a Take Profit Stop loss for the position that is about to be opened? This is when it is necessary to use an order TP/SL (also known as a preset Take Profit stop loss).

In one sentence: Take Profit Stop Loss order is to configure a Take Profit Stop loss at the same time as filling out an open order, and set a Take Profit stop loss for this position when opening a position.

## How is a take profit and stop loss order executed?

The Take Profit stop loss order belongs to the OTO order (One Trigger One). An OTO order is a submission in which the primary order triggers a secondary order.

**1. Submit a Take Profit stop loss order**

When submitting an open order (limit order or market order), check TP/SL and submit a Take Profit stop loss order. The Take Profit stop loss order consists of three orders:

```
1 The main order
2 Order price/market price
3 Quantity
4 Take Profit order
5 Take Profit trigger price
6 Take Profit order price/Market Price
7 Stop loss order
8 Stop Loss trigger price
9 Take Profit order price/Market Price
```

Therefore, in the submission of the take profit stop loss order, in addition to the main order parameters, or the submission of take profit stop trigger price, also require Take Profit stop loss order price and other parameters.

The Take Profit/Stop Loss trigger price must meet the following rules to be submitted:

|                                           | Limit open position                                    | Market open position           |
| ----------------------------------------- | ------------------------------------------------------ | ------------------------------ |
| Open long positions - Take Profit orders  | Trigger price > Min (Main order limit, sell one price) | Trigger price > sell one price |
| Open long positions – Stop Loss order     | Trigger price < Min (Main order limit, sell one price) | Trigger price < sell one price |
| Open short positions - Take Profit orders | Trigger price < Max (Main order limit, buy one price)  | Trigger price < buy one price  |
| Open short positions - Stop Loss order    | Trigger price > Max (Main order limit, buy one price)  | Trigger price > buy one price  |

**2.The Take Profit stop loss order has been submitted and is pending to close**

After the order is submitted, it will appear in 'Current Order', because the principal Take Profit Stop loss order is also a regular order in nature, only with TP/SL information.

For orders in this condition, Take Profit Stop Loss will show 'not in effect', which means that the Take Profit Stop loss order has not been submitted and is waiting for the main order to close.

When the main order is closed, the Take Profit Stop loss will show 'effective', which means that the Take Profit Stop loss order has gone down according to the parameters originally set.

**3.The main order is confirmed and a take profit stop loss order is placed**

When the main order is confirmed and formed in a position with the same order direction, the Take Profit stop loss order is submitted in accordance with the parameters previously set. The quantity of limit take profit stop loss is the number of main orders. Market Take Profit Stop Loss is the exact number of trades.

For example: I submitted a limit order of 1 BTC to buy at $10000, with a Take Profit stop loss. When this order is closed and a position is formed, the system automatically sets a Take Profit stop order with a quantity of 1 BTC for this position, regardless of the number of lots traded on the order. And if I submit a market order for buy open more than 1 BTC, when the market order is closed. Take Profit stop loss orders are set for positions based on the actual number of trades in the order.


**4.Take Profit stop loss orders have been submitted and are awaiting to be triggered**

After a TP/SL order is submitted, the subsequent execution logic is the TP/SL logic of a regular position Take Profit stop loss order.

## Frequently Asked Questions

**Which orders can preset Take Profit Stop Loss?**

Limit open position orders, market price open orders, PostOnly open position orders, IOC open orders, FOK open orders.

**Will subsequent increases in positions also result in a TP/SL for subsequent increases?**

No, the number of limit take profit stop loss is the number of orders (main orders), the number of market trades for TP/SL, and subsequent increases in positions will not take TP/SL.

**What happens when multiple Take Profit stop loss are subsequently placed on the position?**

Take Profit stop loss can hang more than one position, they won’t affect each other, see which one is triggered first.

**What does 'not in effect' mean?**

Take Profit stop loss orders are placed only after the main order is closed and a position is formed in the same direction as the main order. 'Not in effect' means that the placement
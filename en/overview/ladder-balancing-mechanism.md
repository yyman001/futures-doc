# Ladder balancing mechanism

**What is a forced balancing?**

Margin rate is a measure of the risk of position-guaranteed assets, and when the margin rate is close to the minimum maintenance margin rate, the position will be forced to take over by the system. We use the marked price to calculate margin rates to avoid forced closing due to illiquidity or market manipulation.

**About ladder reduction**

In order to prevent large positions from closing when the impact on market liquidity, resulting in large losses, we use a ladder mechanism to reduce positions. Each ladder corresponds to a different maintenance margin rate, when the system determines that the margin is not enough for the current position, it will carry out the operation of reducing the number of positions to the next position.

After the position reaches the strong leveling condition, the system automatically performs the following measures to release the available margin in order to prevent the position from being closed:

* All current orders for this variety contract will be cancelled;
* The long and short positions of the contract with the variety will be traded from the deal;

If the margin rate of the user's position is still less than the current ladder maintenance margin rate after the above steps, a forced reduction operation will be carried out.

* If the margin rate is still < than the current, the system will reduce the position for the purpose of forcing the reduction of positions to the next gear of the net position ceiling, so that the margin rate is greater than 0%;

* If the system calculates that the margin ratio is still not greater than 0% when the mandatory reduction factor is in 1st gear, then all positions will be strongly closed.

When there is a strong trigger, the user cannot carry out this contract-related operations.

Take BTC as an example, when the user has a large position, in gear 3 and above (i.e. the number of positions >=12001, For example: 15000), the burst engine monitors the user's current margin rate is less than or equal to the required maintenance margin rate + closing fee rate, it will not directly close all positions of the users. Instead, the implementation of the mandatory part of the reduction, the first calculation from the current number of positions to reduce the number in 2 gears required to reduce the number of positions = the current number - gear 1 maximum number of positions = 15000-2000 = 13000.

If the user is in restrictive position mode, the system will force the user to hang the number of positions required to reduce the position in accordance with the delegate price slightly better than the latest closing price. During the forced partial reduction period, the user's position in that direction of the contract will be frozen and all contract-related operations will not be possible.

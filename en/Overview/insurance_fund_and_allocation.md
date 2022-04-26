# Insurance fund and allocation

**What is an insurance fund?**

Insurance funds are designed to compensate for losses caused by user positions being lost in particular markets to reduce the likelihood of user funds division.

**How does an insurance fund is created?**

Profits from processing positions after the strong balancing monitor takes over will be injected into the insurance fund.

In the event of strong balancing, the balancing engine will take over the user's position and the remaining margin at the takeover price, if the balancing engine closes the position at a price better than the takeover price, it will generate a profit, this part will be fully injected into the insurance fund.

**How do insurance funds work?**

In the event of strong balancing, the balancing engine will take over the user's position and the remaining margin at the takeover price, if the position continues to lose, the balancing engine closes the position after the loss, this part of the loss is considered to be the system through the position loss, part of the loss will be compensated by the insurance fund, and the remainder will be allocated by the user.

In this exchange contract, all contracts in the same margin currency are shared in the same insurance fund.

**User allocation rules**

After the system is broken, the insurance fund bears part of the loss, the current share of the commitment is 20%, the remaining part (80%) is shared by the user's profit position, which will reduce the user's profit but not lead to loss.


* Filtering rules for profitable positions:

We will count all profitable positions in this settlement cycle and rank these positions profitably, starting with the most profitable positions, and stop looking for the cumulative profit amount, which accounts for 90% of the total profit amount of the settlement system, and the positions found will participate in this allocation. The aim is to avoid the allocation of positions with small profit amounts, only large profit-making accounts are allocated, reducing the long tail of the allocation.

* Fund allocation rules:

The allocation amount of this position= it is the amount of the part of the position to be borne by the user * the profit amount of this position settlement period / the total profit amount of all profitable positions in this settlement period

After the user participates in the allocation, there will be a type of allocated flow of fund liquidity.
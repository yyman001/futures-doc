# Introduction to perpetual contracts
> What is a perpetual contract

**Brief introduction**

A perpetual contract is a futures contract that does not require delivery but can be held permanently. Users can profit from higher/lower prices for digital assets by judging the ups and downs and choosing to buy long or sell short contracts.

**Main points overview**

- Expiration date: Each delivery contract has a fixed due date and the delivery price is the arithmetic average of the US dollar index for the last hour of BTC (LTC, and other coins) as the closing price for all current weekly contracts. The perpetual contract has no expiration date and never expires;


- Capital costs: since there is no expiration delivery date, the perpetual contract needs to be anchored through the "fund fee mechanism" to anchor the exchange price from the contract price;


- Marked price: perpetual contract uses the marked price to calculate the user's unrealized profit and loss, it effectively reduces the market fluctuations when unnecessary liquidation;


- Settlement every minute: through minute-to-minute settlement, the unrealized profit and loss turn into realized profit and loss, it improves the flexibility of the use of funds;


- Ladder Maintenance Margin Rate System: Maintaining margin rate is the minimum margin rate required for the user to maintain his current position. When the margin rate is lower than the maintenance margin rate and the closing fee rate, it triggers liquidation or a partial reduction. For users of different position sizes, the implementation of the ladder maintenance margin rate system, that is, the larger the user's position, the higher the maintenance margin rate, the lower the maximum leverage multiple that the user can choose;


- Force partial balancing: For users with large positions, when the margin rate is lower than the current gear maintenance margin rate + closing fee rate, but higher than the minimum gear maintenance margin rate + closing fee rate, the entire position will not be directly opened. The system will calculate the number of positions required to reduce the position by two gears, and partially reduce the position. After a successful downshift, if the margin rate meets the maintenance margin rate requirements of the new gear, the partial reduction stops, and if the maintenance margin rate requirements of the new gear are still not met, the cycle of partial reduction process will continue. In the position restriction mode, the position is frozen in the process of forced partial reduction, and in the whole position mode, the currency account of the perpetual contract is frozen and cannot be operated in the process of forcing partial position reduction.
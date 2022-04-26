# **Funding Rate**

For the contract on delivery date, the contract market price will return to the index price, the perpetual contract does not expire or gets delivered, the contract price needs to be "capital fee mechanism" to anchor the spot price.

**Collection of funds**

The perpetual contract is settled every 8 hours, at the end of each period, in full hours and 3 times a day, at 00:00, 08:00 and 16:00 respectively. The above times are ALL GMT-8 time.

Only users who hold positions at the time of settlement are required to collect or pay a capital fee, or if the position has been closed before settlement, there is no charge or payment of funds.

At the time of settlement, the user shall charge or pay the capital fee, which shall be determined by the current fund rate and the position of the user. When the fund rate is positive, the long position will pay the capital fee, the short position will charge the capital fee, when the fund rate is negative, the multi-position will charge the capital fee, the short position will pay the capital fee.

Funds are settled entirely between users; the platform does not charge any fees.

**Capital funds calculation**

Capital fee= position value * capital fee rate
The position value= the number of positions * face value * marked price

**The calculation of the capital funds rate**

The capital rate is designed to ensure that the transaction price of the perpetual contract follows the reference price. The funding rates for each period, calculated from the data from the previous period, have been determined at the beginning of the current period, will not change during the period and shall be applied to the settlement of funds expenses at the end of the current period. The forecast funds rate for the next period is also calculated every minute for the current period, and the projected funds rate calculated last in the current period is used as the funding rate for the next period.

If the funds rate for the period 08:00-16:00 is calculated from the data of the previous period 00:00-08:00, it has been determined at 08:00 and used for settlement at 16:00. At the same time, during the period 08:00-16:00, a forecast capital rate is calculated per minute, the fund rate for the period from 16:00 to 00:00 the following day is forecasted, and the last calculated projected fund rate is used as the fund rate for the period from 16:00 to 00:00 the following day.
The capital rate consists of a comprehensive interest rate and a premium.

- Comprehensive interest rates

A perpetual contract consists of two currencies: the underlying currency and the denominated currency. For example: BTCUSDT perpetual contract, the subject currency is BTC, the denominated currency is USDT.

The interest rate in the marked currency: The daily lending rate in the underlying currency in the market. If the subject currency of the BTCUSDT contract is BTC, the underlying currency interest rate is the daily lending rate of the BTC.

Currency interest rate: It is the daily lending rate of the denominated currency in the market. If the denominated currency of the BTCUSDT contract is USDT, the denominated currency interest rate is the daily borrowing rate of the USDT.

Comprehensive Interest Rate (Denominated Currency Rate - The marked Currency Rate) / Capital Rate Settlement Frequency

Currently, all perpetual contracts have a currency rate of 0.06%, the underlying currency rate is 0.03% and the capital rate is settled 3 times (3 times a day). As a result, the combined interest rate for all current perpetual contracts is 0.01%.

II, The premium

A perpetual contract may have a premium or discount relative to its reasonable price. We measure the premium level of a contract by the premium index and add it to the calculation of the capital rate. The higher the premium, the greater the capital rate, the more motivated the sell short side, the lower the premium; the smaller the capital rate, the more motivated the buy long side. By raising or lowering the capital rate, the contract price is brought back to a relatively reasonable level.

* 1-Base rate of funds rate

The base rate of the funds rate reflects the base deviation arising from the current funding costs.

Base rate of funds rate= Current period Fund Rate* ( Current Time Interval / Settlement Period)

If the BTC perpetual contract funds rate for the current period is 0.01%, the current time is 8:30, the current settlement time is 16:00, that is, 7 hours and 30 minutes from the settlement, the settlement period is 8 hours (every 8 hours), then the current funds rate base rate is 0.01% ( 450 / 480 ) . . . 0.009375%

* 2-Reasonable price

The reasonable price is the relatively reasonable reference price of the perpetual contract based on the index price of the current spot and the current base rate of funds rate.

Reasonable price= index price* ( 1 + base rate of funds rate)

If the current BTC index price is $10,000 and the BTC Perpetual Contract base rate of funds rate is 0.005%, the current BTC Perpetual Contract Has a Reasonable Price of 10000 x (1 + 0.005%) = 10000.5 USDT.

* 3-Deep weighted buy/sell price

Deep weighted buy price, refers to according to the current situation of the open order, from the first stage of the purchase, the cumulative volume of pending orders reached is “N” USDT contract average purchase order price.

Deep weighted selling price, refers to according to the current situation of the sale of orders, from the first stage of the sale, the cumulative volume of pending orders reached is “N” USDT contract average selling order price.

Considering an “N” value range of 8000USDT, that would be, Sum (pending order price * number of pending orders) = 8000 USDT

* 1-Premium index

The premium index reflects the current premium situation resulting from the combination of the base rate of the capital rate and the deviation of the deep-weighted buy/sell price from the reasonable price.

Premium Index= [ Max ( 0 , Deep Weighted buy price - Reasonable Price ) - Max ( 0 , Reasonable Price - Deep Weighted Ask Price )] / Index Price + Capital Rate Base Rate;

As can be seen by the formula:

a) When the deep-weighted ask price ≥ reasonable price ≥ deep-weighted buy price, the premium index = the base rate of the fund rate

b) When the depth-weighted ask price > the deep-weighted buy price > reasonable price, the premium index = (deep-weighted bid price - reasonable price) / the index price + the base rate of the fund rate

c) When reasonable price > Deep-weighted ask price > Deep-weighted bid price, premium index = (deep weighted ask price - reasonable price) / index price + funds rate base rate

The premium index is calculated every minute.

* 2- Average premium index

The current average premium index is the arithmetic average of all premium indices for the current period in the last 1 hour.

For the period from 8:00-9:00, the average premium index at 8:30 is the arithmetic average of all premium indices from 7:30-8:30, and the average premium index at 9:00 is the arithmetic average of all premium indices from 8:00-9:00.

Average premium index, calculated every minute.

The forecast of the next funding rate is determined jointly by the composite interest rate and the average premium index. It is based on the following formula:

Forecast next-period capital rate= clamp (average premium index + clamp (comprehensive rate - average premium index, premium deviation from upper limit, premium deviation from lower limit), capital rate cap, funds rate bottom)

In this case clamp is an interval-bound function, only the boundary value is taken when the target value exceeds the upper and lower limits. For example, clamp (a, max, min), when a > max, the result is max, when a < min, the result is min, and when max ≥ a ≥ min, the result is a.

Comprehensive Interest Rate - The average premium index, it is limited between the premium deviation from the upper limit and the premium deviation from the lower limit, and the final forecast of the next fund rate, limited by the capital rate cap and the lower capital rate limit, between the two. The parameters are as follows:


| Premium deviation from the upper limit | Premium deviates from the lower limit | Capital rate cap | Lower limit of the funds rate |
| :------------------------------------: | :-----------------------------------: | :--------------: | :---------------------------: |
|                 0.05%                  |                -0.05%                 |      0.375%      |            -0.375%            |






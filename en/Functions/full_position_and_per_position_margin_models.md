# Full position and restrictive position margin model

**Restrictive position margin mode**

The restrictive position margin model means that the margin of a position is separate from the trader's account balance. In this margin mode, traders are free to determine the multiple of leverage used. If a position is forced to close, the maximum loss that the trader has to bear is the position margin.

**Full position margin mode**

The full position margin model refers to the use of all available balances in the corresponding currency as margin to maintain positions and avoid forced balancing. In this margin mode, a forced close is triggered when the net asset value is insufficient to meet the demand for maintenance margin. If the position is forced to close, the trader will lose all assets in the corresponding currency.

**Adjusting the margin**

Only restrictive position can adjust margin, when adjusting restrictive position margin:

Maximum margin that the user can reduce is= Max (total equity per position - initial margin, 0)

The maximum margin that the user can increase = available

At full position margin, the trader cannot adjust the margin. The system will default to the maximum leverage allowed under the current risk limit to calculate the starting margin.

***Can I switch between full position and restrictive position mode when holding positions?**

No. Margin mode cannot be adjusted when holding positions or pending orders for this contract.
# 全仓和逐仓保证金模式

**逐仓保证金模式**

逐仓保证金模式指的是仓位的保证金与交易者的账户余额是独立分开的。在这种保证金模式下，交易者可以自由决定所用杠杆倍数。如果仓位被强制平仓，交易者所需承担的最大损失即仓位保证金。

**全仓保证金模式**

全仓保证金模式指的是使用相对应币种里所有的可用余额作为仓位保证金来维持仓位，避免强平。在这种保证金模式下，当资产净值不足以满足维持保证金需求时，强制平仓将被触发。如果仓位被强制平仓，交易者将损失所对应币种里所有的资产。

**调节保证金**

只有逐仓仓位可以调节保证金，调节逐仓保证金时：

用户最多可减少的保证金=Max（逐仓总权益-初始保证金，0）

用户最多可增加的保证金=可用

在全仓保证金下, 交易者无法调节保证金。系统将默认使用当前风险限额下所允许的最大杠杆来计算起始保证金。

**持有仓位时，还可以切换全仓与逐仓模式吗？** 不可以。持有本合约仓位或挂单时，无法调节保证金模式。
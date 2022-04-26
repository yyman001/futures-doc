# One-way and two-way positions

**One-way position mode**

In one-way position mode, a contract allows only one position in one direction. When the reverse opening behavior occurs, the existing position is closed before the opening is made.
For example, in a BTCUSDT contract, when you hold a long position of 1 BTC in one-way position mode and open a short position of 2 BTC, your position becomes a short position of 1 BTC.

**Two-way position mode**

In two-way position mode, a contract allows for holding positions in both long and short directions at the same time, and the opening behavior in the opposite direction opens positions in the opposite direction, but positions in the opposite direction do not hedge risks, and when the price moves in one direction, positions in one direction will close.

For example, in a BTCUSDT contract, when you hold a long position of 1 BTC in a two-way position mode and open a short position of 2 BTC, your position becomes a long position of 1 BTC and a short position of 2 BTC.

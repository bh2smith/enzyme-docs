# Protocol Fees

The protocol fee is a 25 bps taxation on the AUM held by a vault in Sulu (v4), the proceeds are burnt to introduce scarcity to **$MLN**.

The way it works, is simple, the fee is accrued in the form of shares, to an Enzyme Council Contract `ProtocolFeeReserveProxy:`

* **Ethereum:** [0xb7460593bd222e24a2bf4393aa6416bd373995e0](https://etherscan.io/address/0xb7460593bd222e24a2bf4393aa6416bd373995e0)
* **Polygon:**  [0xf0bfee2a93b0a1f9c5f6c1d731a6cf1308d68b2d](https://polygonscan.com/address/0xf0bfee2a93b0a1f9c5f6c1d731a6cf1308d68b2d)

The fee is accrued whenever the vault receives a deposit, shares are redeem or a migration/reconfiguration happns.&#x20;

To optimise the ease of fee collection and of passively receiving $MLN to burn, this release uses a shares buyback mechanism:

1. Protocol fee shares are minted at an inflated rate (e.g., 50 bps) above the effective target rate (e.g., 25 bps).
2. Funds can use **$MLN** (i.e., burn) to buy back (i.e., burn) the collected shares at a discount (e.g., 50%).
3. Funds that take advantage of shares buybacks ultimately pay the effective target rate (25 bps) while funds that do not (and leave the Enzyme Council and protocol with the burden of finding other mechanisms for converting shares to $MLN) pay the inflated rate (50 bps).&#x20;

### Auto Buy Back

The Auto Buy Back feature, allows vault managers to automatically buy back protocol fee shares whenever they are collected. For this to work, there needs to be **$MLN** available in the vault, as it will attempt to use the **$MLN** to atomically buy back the full amount of protocol fee shares collected.

To enable the Auto Buy Back feature, please go to **Settings** > **Fees** > **Auto Buyback Protocol Shares** > and click on the button that says "**Enable Shares Buyback**"

You can find more techical details in the [Sulu Specs](https://specs.enzyme.finance/topics/protocol-fee).




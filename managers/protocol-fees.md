# Protocol Access

Accessing the protocol requires MLN tokens: 25 bps taxation on the AUM held by a vault in Sulu (v4).

The way it works, is simple, it is accrued in the form of shares, to an Enzyme Council Contract `ProtocolFeeReserveProxy:`

* **Ethereum:** [0xb7460593bd222e24a2bf4393aa6416bd373995e0](https://etherscan.io/address/0xb7460593bd222e24a2bf4393aa6416bd373995e0)
* **Polygon:**  [0xf0bfee2a93b0a1f9c5f6c1d731a6cf1308d68b2d](https://polygonscan.com/address/0xf0bfee2a93b0a1f9c5f6c1d731a6cf1308d68b2d)

The accrual event happens whenever the vault receives a deposit, shares are redeemed or a migration/reconfiguration happens.&#x20;

To optimise this process, this release uses a shares buyback mechanism:

1. The taxed shares are minted at an inflated rate (e.g., 50 bps) above the effective target rate (e.g., 25 bps).
2. Funds can use **$MLN** to buy back the collected shares at a discount (e.g., 50%).
3. Funds that take advantage of shares buybacks ultimately pay the effective target rate (25 bps) while funds that do not (and leave the Enzyme Council and protocol with the burden of finding other mechanisms for converting shares to $MLN) pay the inflated rate (50 bps).&#x20;

### Auto-Access:

TThe Auto Access feature, allows vault managers to automatically use MLN to access the protocol. For this to work, there needs to be **$MLN** available in the vault.&#x20;

To enable the Auto Access feature, please go to Settings > Fees > Auto Access > and click on the button that says "Enable Auto Access"

You can find more technical details in the [Sulu Specs](https://specs.enzyme.finance/topics/protocol-fee).




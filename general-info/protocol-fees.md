# Protocol fees

The standard protocol is 50bps on Assets Under Technology. However, a reduced rate of 25 bps is applicable when fees are payable in MLN token.

The accrual event happens whenever the vault receives a deposit, shares are redeemed or a migration/reconfiguration happens.

To optimise this process, this release uses a shares buyback mechanism:

1. The taxed shares are minted at an inflated rate (e.g., 50 bps) above the effective target rate (e.g., 25 bps).
2. Funds can use **$MLN** to buy back the collected shares at a discount (50%).
3. Funds that take advantage of shares buybacks ultimately pay the effective target rate (25 bps) while funds that do not (and leave the Enzyme Council and protocol with the burden of finding other mechanisms for converting shares to $MLN) pay the inflated rate (50 bps).

### Other fee models

There are some interesting and innovative new use-cases being built on Enzyme every day. There are cases where the above fee model might not make sense and another fee model will be applied at the discretion of the Enzyme Council.

### Auto-Access:

The Auto Access feature, allows vault managers to automatically use MLN to access the protocol. For this to work, there needs to be **$MLN** available in the vault.

### Auto Buyback Protocol Shares

This option enables you to claim your protocol fee discount in an automated fashion. See fees section for more details about how the fee is applied.

The protocol applies a fee of 50bps on your Assets Under Technology. The fee will be applied by inflating your vault shares. Paying fees with MLN token reduces teh fee to 25bps of your Assets Under Technology.&#x20;

{% hint style="info" %}
Inflated vault shares and MLN collected are unlikely to offer any value to the MLN token given that inflation is likely to exceed the amount burnt for many years to come.
{% endhint %}

By enabling the Auto Buyback Protocol Shares option your vault can take advantage of paying the lower rate of 25 bps all in one transaction.

You’ll need to have $MLN available in your vault to atomically buy back the full amount of protocol fee shares collected during deposits and shares redemption actions.

To enable the Auto Access feature, please go to Settings > Fees > Auto Access > and click on the button that says "Enable Auto Access"

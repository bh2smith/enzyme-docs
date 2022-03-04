# Redeeming

As a depositor into a Vault, you are entitled to withdraw your pro-rata share of that Vault's assets at any time. There is an important nuance to note here, however. Your shares do not entitle you to your pro-rata share of the Vault's assets in the denomination currency unless the vault manager specifies it otherwise in the “**Allowed Assets For Redemption**” policy.

If that is the case, you will be able to redeem the value of your shares in the asset that the vault manager has chosen.&#x20;

As this new redeemable option was just introduced in this latest release, we can expect that old practices may continue. Therefore it is highly probable that when you as a depositor would like to redeem your shares, you may receive a slice of every asset the Vault holds.

{% hint style="info" %}
Let's look at an example. Say you own 1% of the shares outstanding in an Enzyme Vault that's denominated in WETH. Its total assets under management equal 100 WETH, and its portfolio is divided evenly between WETH, WBTC, YFI, and UNI. If you were to redeem your shares, you would receive WETH, WBTC, YFI, and UNI in equal proportions that add up to a total value of 1 WETH. You would not just receive 1 WETH.
{% endhint %}

In either case, to redeem shares, login to your wallet connection provider and click into the Vault's info page. In the top right corner of that page, click the `Redeem` button. This will launch a modal showing your current balance and an input field for you to choose an amount to redeem.

Once you've chosen an amount of shares to redeem, click `Continue`. On the transaction modal that pops up next, confirm the information on the transaction and then click on `Submit`. This will bring up your wallet connection provider asking you to confirm the transaction. Once that's been done, the transaction will be mined and the appropriate token balances will be sent to your wallet.

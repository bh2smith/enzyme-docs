# Redeeming

As a depositor into a Vault, you are entitled to withdraw your pro-rata share of that Vault's assets at any time. There is an important nuance to note here, however. Your shares do not entitle you to your pro-rata share of the Vault's assets in the denomination currency unless the vault manager specifies it otherwise in the “**Allowed Assets For Redemption**” policy.

If that is the case, you will be able to redeem the value of your shares in the asset that the vault manager has chosen.&#x20;

As this new redeemable option was just introduced in this latest release, we can expect that old practices may continue. Therefore it is highly probable that when you as a depositor would like to redeem your shares, you may receive a slice of every asset the Vault holds.

{% hint style="info" %}
Let's look at an example. Say you own 1% of the shares outstanding in an Enzyme Vault that's denominated in WETH. Its total assets under management equal 100 WETH, and its portfolio is divided evenly between WETH, WBTC, YFI, and UNI. If you were to redeem your shares, you would receive WETH, WBTC, YFI, and UNI in equal proportions that add up to a total value of 1 WETH. You would not just receive 1 WETH.
{% endhint %}

In either case, to redeem shares, login to your wallet connection provider and click into the Vault's info page. In the top right corner of that page, click the `Redeem` button. This will launch a modal showing your current balance and an input field for you to choose an amount to redeem.

Once you've chosen an amount of shares to redeem, click `Continue`. On the transaction modal that pops up next, confirm the information on the transaction and then click on `Submit`. This will bring up your wallet connection provider asking you to confirm the transaction. Once that's been done, the transaction will be mined and the appropriate token balances will be sent to your wallet.

{% hint style="danger" %}
If redeeming from a vault that holds external positions, note that redemption in kind can lead to a loss of funds. This option should be disabled on our user interface. If you are unable to redeem from a vault holding external positions, please contact us to discuss other possibilities.
{% endhint %}



## Redeeming through Etherscan or Polygonscan

In the case that the [Enzyme App](https://app.enzyme.finance/) is not available, and you wish to withdraw fund from any vault, you can do so by following these steps



{% hint style="info" %}
You need to previously know your Vault Address. You can get that information on the URL slug in your Enzyme App, or you can find it as the contract creator of the share/token of the vault.
{% endhint %}

\
1\. Search on [Etherscan](https://etherscan.io/)/[Polygonscan](https://polygonscan.com/) for the vault address.

2\. Go to **Contracts**, **More Options** and click on **"is this a proxy?"**

<figure><img src=".gitbook/assets/is this a proxy.png" alt=""><figcaption></figcaption></figure>

3\. A prompt will appear and will be auto-populated, click on **Verify**, and **Save**.

4\. **Click on the link** that is prompted below in a green box.

5\. Then, go to **Contracts**, and select **Read as Proxy**.

6\. Go to item number seven named **`GetAccessor`** and **click on the link** addressed populated below.

7\. Then, go to **Contracts**, **More Options** and click on **“Is this a proxy?”**

8\. A prompt will appear and will be auto-populated, click on **Verify**, and **Save**.

9\. **Click on the link** that is prompted below in a green box.

10\. Then, go to **Contracts**, and **Write as Proxy**.

11\. **Connect your Wallet** to Etherscan/Polygonscan by clicking on the option that says Connect to Web3.

12\. Go to item 17. from the list, named **`redeemSharesInKind`**. Here you will have to specify:

**\_recepient (address):** Your wallet address

**\_sharesQuantity(unit2566):** You will have to convert the number of shares to 18 decimals.&#x20;

{% hint style="info" %}
e.g:

10 share    = 10000000000000000000 > 1 + 19 zeros

1 share    = 1000000000000000000 > 1 + 18 zeros

0.1 share = 100000000000000000 > 1 + 17 zeros
{% endhint %}

**\_additionalAssets(addresses\[]):** here you should add an empty pair of square brackets `[]`

**\_assetsToSkip (address\[]):** here you should add an empty pair of square brackets `[]`

13\. Once that's completed, **click on** **Write**, **and sign the transaction** with the connected wallet.

\



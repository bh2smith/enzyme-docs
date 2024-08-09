# Withdrawals when app not available

In the case that the [Enzyme App](https://app.enzyme.finance/) is not available, and you wish to withdraw fund from any vault, you can do so by following these steps

{% hint style="info" %}
You need to previously know your Vault Address. You can get that information on the URL slug in your Enzyme App, or you can find it as the contract creator of the share/token of the vault.
{% endhint %}

\
1\. Search on [Etherscan](https://etherscan.io/)/[Polygonscan](https://polygonscan.com/) for the vault address.

2\. Go to **Contracts**, **More Options** and click on **"is this a proxy?"**

<figure><img src="../../.gitbook/assets/is this a proxy.png" alt=""><figcaption></figcaption></figure>

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

**\_sharesQuantity(unit2566):** You will have to convert the number of shares to 18 decimals.

{% hint style="info" %}
e.g:

10 share = 10000000000000000000 > 1 + 19 zeros

1 share = 1000000000000000000 > 1 + 18 zeros

0.1 share = 100000000000000000 > 1 + 17 zeros
{% endhint %}

**\_additionalAssets(addresses\[]):** here you should add an empty pair of square brackets `[]`

**\_assetsToSkip (address\[]):** here you should add an empty pair of square brackets `[]`

13\. Once that's completed, **click on** **Write**, **and sign the transaction** with the connected wallet.

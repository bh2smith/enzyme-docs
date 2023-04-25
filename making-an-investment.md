---
description: Depositing to Enzyme Vaults
---

# Making an Investment

Once you've settled on a Vault, you'll need to connect your wallet to the Enzyme app. Click on the `Connect Wallet` button in the top right corner and choose your connection provider.  Metamask, Wallet Connect, Coinbase Wallet and Gnosis Safe are currently compatible; if you do not see your preferred provider, please leave us feedback. We are actively integrating new wallets.

Once you're connected, make sure you've got some of your chosen network's native asset (ETH or MATIC) to pay for gas, then click the `Invest` button in the top right corner of the Vault's page. That will launch a modal that looks like this:

![](<.gitbook/assets/image (44).png>)

You can invest in a vault using ETH or MATIC (depending on which network the vault is on) or the Vault's denomination asset. This is the asset against by which all benchmarks are measured for the Vault's fees. In the case above, the Vault's Denomination Asset is WMATIC. Investing in the vault via the denomination asset is a two step process and requires a transaction for each step.&#x20;

1. Choose an amount to invest and approve it; this transaction grants the vault permission to spend the assets in your wallet
2. Deposit those assets in return for vault shares

After the `Approve` transaction, the modal above should stay open and allow you to execute the `Deposit` transaction. If you navigate away while the `Approve` transaction is processing, clicking the `Deposit` button on the vault page will bring it up again.

You also have the option of investing with the network's native asset (MATIC, in this case, or ETH on mainnet). This requires only one `Deposit` transaction.

Once you've completed either process above and the `Invest` transaction is successfully mined, you are officially a token-holder. The app will take a moment to reflect the changes.

Ownership in Enzyme Vault's is represented by an ERC-20 token that enables you to redeem your shares. You can see an example of one of these tokens [here](https://etherscan.io/address/0x9d4ed905084bbc489a514c75420429c3a246e76d).

{% hint style="danger" %}
Investment in an Enzyme Vault **only** occurs through this two step process. Do not, under any circumstances, send assets directly to the fund contracts. While they will appear in the fund, you will not have a claim on them to redeem.
{% endhint %}

{% hint style="danger" %}
We strongly warn against investing into an Enzyme vault which is allowed to invest in external positions unless you know and trust the manager. This can potentially lead to locked up or lost funds. We recommend you check the policies section on a vault regularly to ensure that no external positions are allowed. We will be introducing automated notifications to alert users of such changes in the near future.

![](<.gitbook/assets/No external positions allowed..png>)
{% endhint %}


# Seed

## What is Seeding?

Seed funding corresponds to the first official funding stage. The purpose of seeding a vault is essentially to get your vault up and running and ready for business.

Let’s say you would like to start your vault with a perfectly balanced portfolio of 25% ZRX, 25% WETH, 25% WBTC and 25% USDC and you already hold those assets. Without seeding, you would have to trade those positions into your denomination asset, deposit into the vault, then trade back into your desired allocations, spending gas on every transaction.

Seeding the Vault with different assets can be more efficient than converting the assets into the denomination asset and back.

**Disclaimer**: we have taken great care to make sure that the procedure described below is accurate. However, we are not responsible for any loss of assets that might occur if you do not follow the procedure as described.

{% hint style="info" %}
Pre-requisites:

* To start with, the Vault has to be empty, i.e. it cannot contain any assets or investments.
* The steps below make use of certain security precautions. It is absolutely vital to follow those precautions as the Vault Manager, otherwise you risk losing all the assets.
* Always double-check all addresses.
{% endhint %}

### **Steps**:

1. Start with a new, empty Enzyme Vault (no assets, no investments).
2. Set up an [**Allowed Deposit Recipients**](investments.md) list with only the Vault Manager (or any other wallet address over which you have control) on the it. This is a crucial security precaution because it prevents a 3rd party from depositing during the seeding phase and claiming ownership of the assets before you do.
3. Confirm that the Enzyme asset universe contains the assets with which you are planning to seed your vault. **IMPORTANT: You can only seed your vault with assets that are already in the Enzyme asset universe. Following the instructions below with assets that are outside the universe may result in permanent loss.** [**A full list of the asset universe can be found here**](https://app.enzyme.finance/network/assets)**.**
4. Find the vault's address. It appears in the URL slug on the Enzyme app, e.g. [https://app.enzyme.finance/vault/{vault-address}/overview](https://app.enzyme.finance/vault/0x86fb84e92c1eedc245987d28a42e123202bd6701/overview). It will begin with `0x`. Make sure that you have the correct address by entering it into Etherscan and confirming that the vault's name appears in the token tracker line of the `More Info` section.
5. Transfer the assets you are using to seed one by one. You can transfer assets directly from your MetaMask or WalletConnect wallet. Keep a portion of the denomination asset in your wallet, you will need to invest this amount into the fund later on.
6. Go back to your vault's [Etherscan](https://etherscan.io/) page and check the `Token` dropdown in the `Contract Overview` section. The assets you have transferred will show up.
7. Add the newly-received assets to your Vault's `tracked assets` list. On your vault page within the Enzyme web app, go to "Settings" => “Assets” => "Add Tracked Assets" and add all the assets that you have transferred, except for the denomination asset (which is always tracked by default).
8. Check that all the assets that you have transferred are correctly shown on the "Overview" page. Please note that it may take several minutes for the asset list to update with the correct amounts.
9. Deposit any amount you like into your Vault (in the denomination asset of your vault). Depositing is a two-step process (approve, deposit). You can deposit using the wallet that you permissioned in step 2.
10. Verify that you have received the shares for the Vault (displayed in the wallet as ENZF, or whatever you have chosen as a token symbol). If you have not received the shares of the Vault, then you might not have completed both steps above. You should now own all the shares of the Vault, and consequently all the assets in the fund.
11. Since fees have been accrued triggered by the first deposit, to start up with a clean vault please make sure to claim all available fees the vault has accrued before proceeding.
12. In order to allow investments by other investors you should add them to the `Limit Wallets Permitted To Deposit` Policy, and with this final step this concludes the fund seeding process.

![This is a slug example](<../../.gitbook/assets/slug\_2 (1).png>)

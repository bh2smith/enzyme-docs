# Assets

![](../../.gitbook/assets/settings\_assets.png)

### **Add Tracked Assets**

Adding tracked assets is a way of telling the protocol to track assets that it doesn’t already know about. By default, new assets are automatically tracked when you trade. However, you may want to add tracked assets to your Vaults which are obtained through other methods such as an airdrop or yield farm. This drop-down allows you to do that.

### Remove Tracked As

If you have added an asset with a zero balance or a balance of less than 0.01 WETH and would like to remove it, you can do so here. However, you cannot remove the denomination asset.

{% hint style="warning" %}
It is important to note that if you are not tracking assets, they will not be reflected in the GAV which may create an arbitrage opportunity for some investors.&#x20;

As a Vault Manager, it is your responsibility to manage these nuances.
{% endhint %}

### **Delegate Trading / Asset Managers**

You may authorize additional addresses to trade on the vault’s behalf. Note that addresses permissioned in this way will have the authority to manage your positions. You can add these permissions and revoke them at a later date.

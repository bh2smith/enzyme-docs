---
description: 'Setup: Step 1'
---

# Vault Basics

The first step of the setup process is simple.

![](<../../.gitbook/assets/image (41).png>)

### **Name**

Although each Vault on Enzyme is identified by its own unique Ethereum address, it is also possible to choose a name for it. It is possible for more than one product to have the same name so you might want to check that the name you have in mind hasn't been used before.

### Symbol

This is the symbol of your vault's shares (which are ERC-20 tokens). It defaults to ENZF, but you can change it to personalize as you see fit.&#x20;

### Denomination Asset

The denomination asset is the base asset of your Vault. There are several implications to think about when choosing a denomination asset.

* **Performance Fees**[**\***](fees.md)**:** It is the asset that your Vault's **performance fee** will be benchmarked and calculated against.&#x20;
* **Deploying capital:** It is the asset that will be received from subscribers to your Vault and therefore the asset that will be held by the product's portfolio before you deploy it.&#x20;
* **Synthetix:** If you plan to use Synthetix heavily, you will need sUSD or sETH to enter in and out of most synth positions. It likely makes sense for you to denominate your product in sUSD for simplicity, security and lower costs ([see risks & nuances section](https://userdocs.enzyme.finance/risks)).

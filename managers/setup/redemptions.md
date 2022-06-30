---
description: 'Setup: Step 5 (Redemptions settings can be changed after creation)'
---

# Redemptions

Generally speaking, deposits to and redemptions from your Vault are possible 24/7 unless you add a policy that dictates otherwise. **Caveat:** Trading heavily on Synthetix or other similarly designed exchanges, and the use of external positions may occasionally make redemptions not possible because of their delayed settlement design. The Guaranteed Redemption Policy ensures that your Vault has a policy that restricts you from trading during a specific time period each day so that depositors know with certainty that they can redeem within this window. This is a recommended policy to have if you will be trading with Synthetix. If you have any questions about using this policy, come and [discuss](https://t.me/enzymefinance) them with us.

![](<../../.gitbook/assets/redemptions (1).png>)

## **Restrict Assets For Redemption**

Restricts the assets for which a depositor may redeem their vault shares. If this [policy](https://docs.enzyme.finance/managers/setup/redemptions) is not enabled, depositors may redeem their shares in-kind or in any arbitrary combination of assets held by your vault. There are two common implementations of this policy to control how your depositors can redeem their shares:

1. To limit depositors' redemption options to **in-kind** or **specific-asset** redemptions where you control which assets are available, toggle this policy on and add assets to the list. Note that if you use this implementation, your depositors can materially change the composition of your portfolio without notice. Implementing an accompanying Single Asset Redemption Threshold (below) can mitigate this risk.
2. To limit depositors' redemption options to **in-kind** only, toggle this policy on, toggle 'Only allow in-kind redemption' on, and leave the list of assets empty.

## **Specific Asset Redemption Threshold**

Restricts the value of a single-asset redemption by setting a minimum balance of that asset that the vault must maintain post-withdrawal. Single-asset withdrawals that would reduce the vault's balance below this level will be rejected. Note that the depositor can still redeem their shares by withdrawing their pro rata share of the vault's holdings.

## **Shares Lockup-Up Period**

Defines the amount of time that must pass from the time a user deposits until they’re allowed to either redeem or transfer any shares. This is arbitrage protection, and funds that have untrusted depositors should use a non-zero value. Depending on the trust level between the Depositors and the vault Manager, we recommend at least a 24 hours lock-up period.

****

****

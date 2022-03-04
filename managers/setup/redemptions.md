---
description: 'Setup: Step 5 (Redemptions settings can be changed after creation)'
---

# Redemptions

Generally speaking, deposits to and redemptions from your Vault are possible 24/7 unless you add a policy that dictates otherwise. **Caveat:** Trading heavily on Synthetix or other similarly designed exchanges, and the use of external positions may occasionally make redemptions not possible because of their delayed settlement design. The Guaranteed Redemption Policy ensures that your Vault has a policy that restricts you from trading during a specific time period each day so that depositors know with certainty that they can redeem within this window. This is a recommended policy to have if you will be trading with Synthetix. If you have any questions about using this policy, come and [discuss](https://t.me/enzymefinance) them with us.

![](<../../.gitbook/assets/image (43).png>)

## **Shares Lockup**

Defines the amount of time that must pass from the time a user deposits until they’re allowed to either redeem or transfer any shares. This is arbitrage protection, and funds that have untrusted depositors should use a non-zero value. We recommend 24 hours.

## **Allowed Assets For Redemption**

This enables a vault's depositors to redeem their shares in a single asset. You can define the asset(s) that are allowed to be included in specific asset redemption.

## **Single Asset Redemption Threshold**

Restricts the value of a single-asset redemption by setting a minimum balance of that asset that the vault must maintain post-withdrawal. Single-asset withdrawals that would reduce the vault's balance below this level will be rejected. Note that the depositor can still redeem their shares by withdrawing their pro rata share of the vault's holdings.

## **Guaranteed Redemption Period**

This policy ensures that the vault will have a fixed daily time period during which depositors will be able to freely withdraw their shares or deposit more. During that period, the vault cannot trade on Synthetix which makes the guarantee possible.

****

# Risks and Nuances

## 24/7 Redemption: Caveats

Generally speaking, you are always in control of the shares you buy in Enzyme products and can redeem them at any time. Occasionally however, some edge cases arise because of the way that some DeFi protocols work. For example, Synthetix typically uses a delayed settlement time of 180 seconds. Further complicating matters, this settlement time is an adjustable parameter by Synthetix governance. In this release, we have introduced the concept of external positions, which is another tool for managers to diversify their strategies. However, in this scenario and the scenario previously described, if a subscriber tries to redeem shares from an Enzyme product that's just made a trade on Synthetix but before that trade has settled, or has an External Position, they will not be able to.

If guaranteed 24/7 redeemability is a condition required for you to invest into a product, you should check the product configurations on the product's page to make sure that Synthetix is on the **adapter blacklist** (ie. Portfolio Manager can never trade on Synthetix) **and that the vault is not allowed to open External Positions**. It is important to check that this condition still holds at the time when any upgrade is signaled by a Portfolio Manager.

In an extreme edge case, a Portfolio Manager might be trading Synthetix heavily in which case you will might not have the chance to redeem as often as they would like. If this concerns you, you should look to invest in products which have a Guaranteed Redemption policy. More information can be found on this policy in the Redemptions section. Note that it is your responsibility to check this policy still holds during an upgrade period.

## Migrations

Enzyme is constantly adding new features and integrations with external decentralised finance protocols. Occasionally, these features will require a new release of the core Enzyme contracts. Investors should be aware that at every new Enzyme release, Portfolio Managers can opt in to upgrade their product from the previous version to the new version. This process gives Portfolio Managers an opportunity to change their original product configurations (eg. fees, rule-sets, etc). Once the product configurations are updated and the Portfolio Manager has signaled their intent to migrate to the new Enzyme version, the Portfolio Manager is restricted from accessing the upgrade for 7 days. This time period gives investors an opportunity to opt out of the product by redeeming their shares.

{% hint style="info" %}
At every release cycle, investors should regularly check the product configurations they are subscribed to in order to make sure they still agree to them.
{% endhint %}

In order to make this monitoring of events more user friendly, we will be releasing notification services for users in the coming months. In the meantime, any Enzyme upgrades will be well-publicised [here](https://twitter.com/enzymefinance), [here](https://twitter.com/avantgardefi), and [here](https://t.me/enzymefinance).

## Smart Contract Risk

Enzyme takes security very seriously. Any publicly-available Enzyme code has been thoroughly audited; the results are available for anyone to read[ here](https://audit.enzyme.finance). However, when interacting with any smart contract protocol, there is always some degree of risk that an edge case or code vulnerability can result in funds being lost. Investing funds into an Enzyme product is an acknowledgement and acceptance of this risk.

For any questions about these risks, our team is always happy to [help](https://t.me/enzymefinance).

## Oracle Risk

Enzyme relies on oracles to calculate the gross asset values of any investment product. If these oracles are compromised in any way, they can provide attack vectors to users which could lead to a loss of funds.

## Asset Risk

It is the Portfolio Manager to stay on top of any nuances surrounding tokens. The available asset universe is not intended to be any list of endorsement. Things to look out for could include the risk of token migrations, deviations from the ERC-20 standard, the degree of centralised custodial risk (eg. USDT) and how prices are derived (for example, we use the BTC/ETH rate for WBTC).&#x20;

## Farming Rewards

Make sure you are using a Vault manager who understands the nuances of farming. When a Vault manager has unclaimed tokens, that Vault potentially becomes a target for arbitrageurs (at the expense of other depositors in the Vault). Typically its a good idea to make sure that a Vault which does farm, uses some kind of preventative measure (eg. a whitelist or an entrance fee) to deter such behaviour.

## External Positions

A vault that uses external positions requires substantially more trust in that vault's manager than other adapters. This is because redemptions might not always be possible if the Vault’s assets are tied up in external positions.

If you are depositing into a vault which is able to hold external positions, make sure that you take the necessary steps to know who the vault manager is and establish trust between you.

It is possible for a manager to upgrade a vault to allow for external positions. This would entail a seven day cool-off period before the new changes take effect. We recommend you check the settings regularly to ensure this is not possible. We will be introducing automated notifications to alert users of such changes in the near future.

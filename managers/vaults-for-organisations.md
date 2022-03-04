---
description: DAOs, companies etc
---

# Vaults for DAOs & Organisations

Until recently, Enzyme has primarily catered to single Vault Managers owning an Ethereum wallet. This section explores how to create Enzyme products with organisations using Gnosis Safe.

## What is Gnosis Safe?

Gnosis Safe is a multisig wallet which allows organisations to customize how they manage their crypto assets, with the option to require a predefined number of signatures to confirm transactions before they are executed. This helps prevent unauthorized access to organisation-owned crypto.

## **Why Gnosis Safe + Enzyme?** <a href="#b545" id="b545"></a>

You might be asking yourself why would anyone want to use a multisig to manage assets with Enzyme? Here are a few reasons:

* Organisations are able to access a quick & easy way to connect to multiple DEX trading venues (eg. DEXs, aggregators, derivatives), DeFi protocols (eg. depositing to AMM pools, lending) and DeFi benefits (eg. farming or airdrops) _**from**  **one**  **place**._
* Enzyme provides users with full, easily readable, auditable and transparent reporting over assets being managed.
* Organisations can delegate trading to 3rd-party for efficiency in a non-custodial way (and revoke it at any time). The 3rd party can also be a trading bot.
* Organisations can pull in outside investors to invest alongside their strategies and charge optional fees (eg management, performance, entrance all calculated and distributed in an automated way).
* Gnosis Safe gives Vault managers a way to layer organisational governance structures on top of their products.

Let’s explore a few concrete use-cases that might be interesting:

### **1. DAO Treasury Management** <a href="#89e1" id="89e1"></a>

DAOs often sit on large treasuries which are not being actively managed. It can be challenging to manage a DAO treasury efficiently and track its performance transparently. This is a perfect use-case for Gnosis Safe + Enzyme. Organisations can simply plug their Gnosis Safe into Enzyme and engage with a purpose-built asset management toolkit.

### 2. Crypto Investment Clubs

Investment clubs are groups of individuals who join together to invest together and share resources. In many countries they also benefit from regulatory exemptions. Members of such clubs typically meet on a periodic basis to make investment decisions as a group through a voting process and recording of minutes, or gather information and perform investment transactions. A combination of Gnosis Safe + Enzyme enables you to set one of these up in minutes!

### **3. Eliminating Operational Risk** <a href="#5068" id="5068"></a>

In general, nobody likes operational risk — especially organisations. If a Vault Manager were to compromise his/her private key or become incapacitated there is a question over what happens to the future of their assets. By having a multisig, you can drastically reduce these kinds of operational risks.

The possibilities are endless, those are just a few common use cases of a multisig on Enzyme.

## **Getting started** <a href="#3175" id="3175"></a>

### **Step 1: Connect to Enzyme with a multisig.** <a href="#7f3a" id="7f3a"></a>

If you don’t already have a multisig safe, go to the [Gnosis Safe app](https://gnosis-safe.io/app/#/welcome) and follow the instructions to set up your Safe. If you already have one ready, just load it up from the Gnosis app.

Once you’re set up with your Safe, click on Apps -> Wallet Connect.![Image for post](https://miro.medium.com/max/3200/0\*z95AhyUinRM09Fci)

![](https://miro.medium.com/max/60/0\*z95AhyUinRM09Fci?q=20)

Now go to the [Enzyme App](http://app.enzyme.finance) and connect using Wallet Connect. You’ll see a QR code pop up which you need to copy to clipboard. Now go back to the Gnosis Safe page and paste the QR code into the wallet connect box highlighted in the image above.

You’re now connected to Enzyme with your multisig!

### **Step 2: Setting up with Enzyme.** <a href="#7fae" id="7fae"></a>

If you go back to the [Enzyme app](http://app.enzyme.finance) now, you’ll see you are connected with your multisig wallet! You can now start plugging your organisation into Enzyme. Make sure you are on the “For Vault Managers” launchpad and click “Create”. If in doubt, you can refer to our [user docs](http://userdocs.enzyme.finance) here or [contact us](https://t.me/enzymefinance).

### **Step 3: Deploying your Enzyme vehicle** <a href="#bba8" id="bba8"></a>

Once you’re done creating your organisation’s connection to Enzyme, you will get prompted to sign a transaction. Submit the transaction and then go back to the Gnosis Safe App. Make sure you are logged in with one of the **multisig** **Owner** addresses and connect with Wallet Connect. It should prompt you to sign a transaction. Now keep repeating this process with other **multisig Owners** until you’ve passed the signing threshold. At that point, your Enzyme vehicle should be deployed on-chain and visible on the Vault Manager launchpad. For more information on what you can do with Enzyme, this might be a good time to [refer our user docs](http://userdocs.enzyme.finance).

### **Step 4: Delegate trading** <a href="#6d43" id="6d43"></a>

It can be slow and inefficient to pass the multisig threshold every time you need to do a trade or interact with a DeFi protocol on Enzyme. So we’ve come up with a way to delegate trading to one address. The owner of this address can be a bot, a company’s trader or an assigned group delegated by a DAO. The interesting thing about this permission is that it only gives permissions for trading and that permission can be revoked any time by the organisation.![Image for post](https://miro.medium.com/max/60/0\*nWEBVxG6D\_\_7Zl9k?q=20)![Image for post](https://miro.medium.com/max/3200/0\*nWEBVxG6D\_\_7Zl9k)

In order to delegate trading to one (or more) addresses, go the Settings tab from the Vault Manager Launchpad and scroll down until you see Delegate Trading. Enter the Ethereum address and Add User and submit the transaction. Now just go back to the Gnosis Safe app and repeat the steps provided earlier. Ask the multisig owners to log in with their address, connect via Wallet Connect and sign the pending transaction.

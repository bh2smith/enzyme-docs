# Depositing Into Diva Vaults

### Where can I find the official T\&Cs for the Early Stakers Initiative?

The official reference is [DIP-02](https://www.tally.xyz/gov/diva/proposal/45468458207916765916984557235161596151150976178275597160417224501662414206717), which was voted and approved by the DAO.

### What is the official page of the program?&#x20;

The official URL is [diva.enzyme.finance](https://diva.enzyme.finance/).&#x20;

### Can I deposit by sending assets directly to the vault address?

No. Deposits shall be made following the Enzyme UI without sending funds directly to the vault address. Funds sent directly to the address would not mint new vault shares for the depositor so the value would be "airdropped" to the current shareholders and therefore lost by the depositor.&#x20;

<figure><img src="https://lh4.googleusercontent.com/YY0OnXDbOds19lfsouwuwebklZ0XUoYcVmLT0v7CIhd5KTRUwwET-WY2NldZ9Ezk09wmtvfJIkqPu5hcpXo96e7e9Hkpn75DgLvDcZfbnW2RpbDKC2AQPsXaCLRoAgn3fjDxJvvVo-QAOjFDhXSmc48" alt=""><figcaption></figcaption></figure>

### Where can I send my questions if the FAQ does not cover my doubts or if I have a technical issue to troubleshoot?

You can send an email to diva@enzyme.finance. You’ll receive an answer within 24h. In case of technical issues, please consider adding the following details:&#x20;

* Wallet address used for deposit.
* Type of wallet (e.g., Metamask, Gnosis, Ledger).
* Connection method (e.g., via WalletConnect, Ledger through Metamask).
* Steps you took when the issue occurred.
* Any screenshots of the error you witnessed.

### Where can I follow the progress of the initiative in terms of TVL?&#x20;

You can see the TVL on the [stETH vault here](https://diva-steth.enzyme.community/vault/0x1ce8aafb51e79f6bdc0ef2ebd6fd34b00620f6db?currency=ETH)

You can see the TVL on the [ETH vault here](https://diva-eth.enzyme.community/vault/0x16770d642e882e1769ce4ac8612b8bc0601506fc?currency=ETH)

### I can’t sign the special T\&Cs with my Gnosis Safe. How do I do it?

If your Safe is doing on-chain signatures, it will not work. You will need to do off-chain signatures. You should be able to change this in “Settings” -> “Safe Apps” -> “Signing Method”, which should be left unchecked. \


<figure><img src="https://lh3.googleusercontent.com/2M0vLyDpjQ3-ptO8-KjEpzNXlV2foOl58j7IyvKzFdc2W3PIO20aXbf3id2_i9Khvaf9aobcmcttVbUktn-lD5M6K30khUUPPGWrtPaFJZ5uEvpW_f093PptEixOSoKBP8qk67CBpyjAu0NsKPk4obc" alt=""><figcaption></figcaption></figure>

### Where/how do we see how much DIVA I have accrued so far?

As you can also see from the T\&Cs approved on [DIP-02](https://www.tally.xyz/gov/diva/proposal/45468458207916765916984557235161596151150976178275597160417224501662414206717), the accrual of DIVA won't start until 30 days prior to mainnet launch. Since that date is still to be determined, the accrual will be accounted as a 30-day lookback from the launch date. As the launch date approaches, we'll&#x20;

see how we can hook up our API with a dashboard that gives each staker a personalised overview of the DIVA accrued to date. Since rewards (i.e. DIVA/ETH/Day) are decreasing as TVL grows, today's deposits are useful to lock in the highest tier.&#x20;

### Why do I see ETH as an option for deposit on the stETH vault?

The stETH denominated vault accepts stETH deposits (kinda obvious) but also ETH deposits. In case someone comes with ETH, the protocol automatically converts ETH into the denomination asset during the deposit process, using Paraswap. In other words, you don't have to convert/mint stETH yourself and the asset that lands on the vault is always the denomination one. This is a standard of the Enzyme architecture across all vaults.

### Is there any difference between the 2 vaults in terms of DIVA rewards?

No. DIVA rewards will be the same for both vaults. The only difference is that the stETH vault will keep earning you staking rewards through the LST rebasing mechanism on top of DIVA incentives.&#x20;

### Why am I not getting 1:1 DSTVL vault shares with my stETH deposit?

That's because as time goes by the vault starts to accrue rebasing ETH staking rewards on the pre-existing AUM so the vault share DSTVL starts to appreciate relative to stETH in a non-rebasing manner. A good example of this is the Unslashed Finance [vault](https://app.enzyme.finance/vault/0x86fb84e92c1eedc245987d28a42e123202bd6701?currency=ETH), where you can see the share appreciation over time as a result of stETH rewards.

\
\
\

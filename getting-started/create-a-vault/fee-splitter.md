# Fee Splitter

The Fee Splitter is a newly introduced Enzyme feature that allows you to split your fees among several wallets.

#### Use cases <a href="#use-cases" id="use-cases"></a>

Shared asset management: you are sharing the effort of the management with another DeFi strategist and want to split fees with them.

Commercial partnerships: you have a person who is facilitating the onboarding of new depositors and you agree on a certain reward based on new AUM or future performance.

Distribution network: you have a network of allocators/distributors that are cooperating in the success of the DeFi strategy and you want to systemise the fee distribution.

#### How to enable the Fee Splitter <a href="#how-to-enable-the-fee-splitter" id="how-to-enable-the-fee-splitter"></a>

The fee splitter is one of our enhanced features so if you are interested in using the Fee Splitter, please reach out our team via email to support@avantgarde.finace

#### How to create a Fee Splitter <a href="#how-to-create-a-fee-splitter" id="how-to-create-a-fee-splitter"></a>

1\. After reaching out to the Avantgarde Finance team, you will be provided with a link where you can create your own Fee Splitter.

2\. On the top right corner, click on “+ Create fee splitter”.

3\. Add all recipient wallets, specifying the % distribution for each wallet. Note that the total sum must always be 100%. You can split fees up to a maximum of **10 different wallets**.

<figure><img src="https://docs.enzyme.finance/~gitbook/image?url=https%3A%2F%2F2049782695-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWzXrybpj5e9VBbPlbYCJ%252Fuploads%252FQbdv42RHjc3fqZdbP3JU%252F1.png%3Falt%3Dmedia%26token%3D42210c05-aa21-40a6-a6a9-0b343069a8a7&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=f6ad8c2f&#x26;sv=1" alt=""><figcaption></figcaption></figure>

4\. Once you execute the transaction, the splitter will provide you with a contract address.

<figure><img src="https://docs.enzyme.finance/~gitbook/image?url=https%3A%2F%2F2049782695-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWzXrybpj5e9VBbPlbYCJ%252Fuploads%252FyTWCFzrLzzTSOQeaIPB9%252F2.png%3Falt%3Dmedia%26token%3D8d6c6ab5-937d-471c-b5d9-f99815b8a63e&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=385416e&#x26;sv=1" alt=""><figcaption></figcaption></figure>

#### How to connect the Fee Splitter to your vault <a href="#how-to-connect-the-fee-splitter-to-your-vault" id="how-to-connect-the-fee-splitter-to-your-vault"></a>

**For existing vaults**: to enable the fee splitter you will need to go to Settings > Fees and Fee Splitter. Copy the new address and paste it as the sole recipient of the management, performance, entrance or exit fees. Upon distribution/claim of the fees, the contract will automatically pay out using the underlying pro-rata split.

<figure><img src="https://docs.enzyme.finance/~gitbook/image?url=https%3A%2F%2F2049782695-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWzXrybpj5e9VBbPlbYCJ%252Fuploads%252FitQ3qPRBrNyL6Y7OeyPL%252F3.png%3Falt%3Dmedia%26token%3D7baa1b47-5d3d-4347-81f5-d3527628b1c8&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=ed656003&#x26;sv=1" alt=""><figcaption></figcaption></figure>

**For new vaults**, it is easier. We recommend creating the fee splitter contracts first, and then proceeding with the vault creation. As you define vault fees, you’ll need to set the contract address as the only recipient address.

<figure><img src="https://docs.enzyme.finance/~gitbook/image?url=https%3A%2F%2F2049782695-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWzXrybpj5e9VBbPlbYCJ%252Fuploads%252FM6XRAhmr9oKQjNlFrrAA%252Fimage.png%3Falt%3Dmedia%26token%3Df207cd24-7e07-432c-8db3-66bb5c0fd68e&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=727b4b87&#x26;sv=1" alt=""><figcaption></figcaption></figure>

In case you manage several vaults with identical configurations, bear in mind that the splitter contract **can be reused** for more than one vault.

#### How to claim fees <a href="#how-to-claim-fees" id="how-to-claim-fees"></a>

<figure><img src="https://docs.enzyme.finance/~gitbook/image?url=https%3A%2F%2F2049782695-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWzXrybpj5e9VBbPlbYCJ%252Fuploads%252FRmlUldzpx2fkeJdI6WwZ%252Ffee_splitter.png%3Falt%3Dmedia%26token%3D32c21cb2-0827-462e-b87a-14437e800fec&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=1c1c8a35&#x26;sv=1" alt=""><figcaption></figcaption></figure>

Any beneficiary of the fee recipient needs to go to the fee section of the vault, and click on claim fees.

You need to be logged in with the address of the fee recipient.

#### **How to update the Fee Splitter** <a href="#how-to-update-the-fee-splitter" id="how-to-update-the-fee-splitter"></a>

The fee splitter contract **cannot be updated,** so if you want to change the percentages or add/remove addresses you will need to create a new contract and replace it in your vault settings.

Are you ready to start using the Fee Splitter? Send us your request at **support@avantgarde.finance**.

# Vault Types

In this release, we have introduced different vault types, with different preset policies to reflect the varying levels of trust that exist or are perceived between the manager and investors.&#x20;

Different vaults are created for different purposes with different trust relationships, thus we have pre-configured policies to easily create vaults without going through each individual policy.

![](<../../.gitbook/assets/vault types.png>)

### Public Vault - Trusted Vault Owner

This vault requires Depositors to trust in the Vault Owner.  Usually this will be a known party and legal documents might be involved.

### Private Vault

This is a vault with full trust, where Depositors trust the Vault Owner and vice versa. Typically there will be an "allowed depositer" list on this type of vault, possibly a KYC and likely some legal documents to define the relationship.

### Public Vault - Trustless

In this vault, trust does not need to exist between Depositors and the Vault Owner. The contract configurations should be enough to protect investors from malicious behaviour and vica-versa. Certain activities or features might not be allowed from this type of vault.

### Start From Scratch

If you chose this option, we will not be suggesting any pre-set policy configuration so you can explore the policies and customize your vault to what you need.



More on this topic can be found [here](https://medium.com/enzymefinance/fifty-shades-of-trust-25642aab3079).

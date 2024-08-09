# \*Restrict Asset Position Removal

This policy exists to protect against a delegated trader un-tracking an asset in the vault such that it is no longer being accounted for. This can create incorrect valuation of vaults and we recommend reading about the risks this causes in the [risks & nuances](https://app.gitbook.com/o/-M17sAWG26bbHj7WurKa/s/WzXrybpj5e9VBbPlbYCJ/\~/changes/238/general-info/risks-and-nuances) section.

This policy prevents the removal of an external position from the vault’s accounting unless its value can be considered negligible (i.e. dust). The dust threshold is maintained by the Enzyme Council.

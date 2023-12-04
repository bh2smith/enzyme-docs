# Background

## Brief History

Enzyme has [rebranded](https://medium.com/enzymefinance/from-melon-to-enzyme-b5b56512f40d) from Melon Protocol. The protocol has been on mainnet since Feb 2019 and was the first DeFi protocol to decentralise its governance. Enzyme v2 was launched to mainnet in Jan 2021 and is a completely re-architected protocol with modularity and extensibility at the core of its design.

## Enzyme Token

Enzyme’s token is [MLN](https://etherscan.io/token/0xec67005c4e498ec7f55e092bd1d35cbc47c91892) and has a dual use:

1\) enables access the MLN network.

2\) used to incentivise developers to build on Enzyme.

## Enzyme Protocol Fee

This release implements a protocol fee, which is charged by minting additional vault shares to an Enzyme Council owned contract.

Initially applied at 50 bps of AUM but can be bought back by the vault manager for 25 bps.

The Enzyme Council owned shares can be bought back in the equivalent value of $MLN,  by the vault manager at 25 bps. The $MLN is then burned. The “50% discount” encourages the vault manager to take care of this process rather than the Council having to.

The protocol fee is charged each time that a fund:

* receives a new deposit
* has shares redeemed
* migrates to a new release or reconfigures vault settings without migrating

A more detailed discussion of the mechanics of the protocol fee can be found [here](https://avantgarde-finance.gitbook.io/enzyme-protocol-v4-sulu-general-spec/topics/protocol-fee).

## Governance

Enzyme is governed by a DAO known as the Enzyme Council which is made up of technical experts and user representatives. A complete discussion of the protocol's governance can be found [here](https://avantgarde-finance.gitbook.io/enzyme-protocol-v2-general-spec/governance/overview).

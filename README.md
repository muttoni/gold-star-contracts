# Gold Star Cadence Contracts

A non-exhaustive list of interesting Cadence contracts, scripts, transactions and what makes them great. 

## Contracts

### Foundational Interfaces
These contracts are so-called foundational because they are standard interfaces that any FT or NFT contract will implement. They introduce commonly seen resources such as Vaults, Collections as well as standard events.

- [FungibleToken Interface](https://github.com/onflow/flow-ft/blob/master/contracts/FungibleToken.cdc) - Example implementations: [FlowToken](https://flow-view-source.com/mainnet/account/0x1654653399040a61/contract/FlowToken), [FUSD](https://github.com/onflow/fusd/blob/main/contracts/FUSD.cdc)
- [NonFungibleToken Interface](https://github.com/onflow/flow-nft/blob/master/contracts/NonFungibleToken.cdc) - See below for implementations

### Mainnet
An collection of contracts currently deployed on mainnet that show Cadence best practices and worth studying (in alphabetical order).

#### [.find](https://github.com/findonflow/find/tree/main/contracts)

[Find](find.xyz) is a name service for Flow. It has contracts showing how to implement Profiles, Donations, displaying user's various NFTs (although things will change in the near future with the NFT Metadata standard) as well as how the .find name service works from a Smart Contract level. 

#### [NFT Storefront](https://github.com/onflow/nft-storefront/blob/main/contracts/NFTStorefront.cdc)

The NFT storefront is a general-purpose Cadence contract for trading NFTs on Flow.

NFTStorefront uses modern Cadence [run-time type](https://github.com/onflow/nft-storefront) facilities to implement a marketplace that can take any currency in order to vend any token in a safe and secure way. This means that only one instance of the contract is needed (visit link for its address on Testnet and Mainnet), and its resources, transactions, and scripts can be used by any account to create any marketplace.

## Contributing 

If you would like to add your contracts to this list, please add a new folder in this repo with the your contract(s) and an explanatory markdown walkthrough that explains the contract's interesting bits, and why it is worth studying.

```
your-project-name/
├─ your-contract(s).cdc
└─ walkthrough.md
```


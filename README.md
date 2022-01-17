# Gold Star Cadence Contracts

A non-exhaustive list of Cadence contracts, scripts, transactions that exemplify best practices. 

## Contracts

### Foundational Interfaces
These contracts are so-called foundational because they are standard interfaces that any FT or NFT contract will implement. They introduce commonly seen resources such as Vaults, Collections as well as standard events.

- [FungibleToken Interface](https://github.com/onflow/flow-ft/blob/master/contracts/FungibleToken.cdc) - Example implementations: [FlowToken](https://flow-view-source.com/mainnet/account/0x1654653399040a61/contract/FlowToken), [FUSD](https://github.com/onflow/fusd/blob/main/contracts/FUSD.cdc)
- [NonFungibleToken Interface](https://github.com/onflow/flow-nft/blob/master/contracts/NonFungibleToken.cdc) - See below for implementations

### Mainnet
An collection of contracts currently deployed on mainnet that show Cadence best practices and worth studying.

#### [Flow Core Contracts](https://github.com/onflow/flow-core-contracts)
The core smart contracts powering the Flow Blockchain. 

#### [USDC Contract](https://github.com/flow-usdc/flow-usdc)
An implementation of the CENTRE Fiat Token in Cadence, on the Flow Blockchain. Shows a good example of a `FiatToken`, which implements interfaces `FungibleToken`, `FiatTokenInterface`, and `OnChainMultiSig`. 

#### [NFT Storefront](https://github.com/onflow/nft-storefront/blob/main/contracts/NFTStorefront.cdc)

#### [Chainmonsters](https://github.com/bsidegames/chainmonsters-smart-contracts)

Each [Chainmonsters](https://chainmonsters.com/) NFT represents a Chainmon, item or cosmetic from within the game. The NFTs are grouped into seasons which usually have some overarching theme, exclusive items and rewards. Multiple NFTs can be minted from the same reward and each receives a serial number that indicates where in the edition it was minted.

#### [.find](https://github.com/findonflow/find/tree/main/contracts)

[Find](find.xyz) is a name service for Flow. It has contracts showing how to implement Profiles, Donations, displaying user's various NFTs (although things will change in the near future with the NFT Metadata standard) as well as how the .find name service works from a Smart Contract level. 

The NFT storefront is a general-purpose Cadence contract for trading NFTs on Flow. NFTStorefront uses modern Cadence [run-time type](https://github.com/onflow/nft-storefront) facilities to implement a marketplace that can take any currency in order to vend any token in a safe and secure way. This means that only one instance of the contract is needed (visit link for its address on Testnet and Mainnet), and its resources, transactions, and scripts can be used by any account to create any marketplace.

#### [Versus](https://github.com/versus-flow/versus-contracts)

[Versus](https://versus.auction) is a novel auction style NFT marketplace. Its contracts show good examples of implementing the NFT interface as well as how to setup an auction style marketplace.

### Testnet

#### [Kitty Items](https://github.com/onflow/kitty-items)

## Contributing 

If you would like to add your contracts to this list, please submit a PR following the pattern above – i.e. link to contract and explanation as to why it's worth studying/learning from.




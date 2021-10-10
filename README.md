# sharedtools-index
Sharedtools repo and contract index for ETHOnline2021

## Overview: 
![architecture overview](https://docs.google.com/drawings/d/e/2PACX-1vSdmv2G1qHZKdaX3aobWG1crxlhS0BHgCoHMGzadL34rxXuKOmDactqgXzU6djn1VqGG172aoD6-d8k/pub?w=1235&h=760)


## Writings:
- Article / mission statement:
  https://medium.com/@chimera_defi/sharedtools-c2fe8e49ba9b
- Presentation:
 https://docs.google.com/presentation/d/1R50pb8qXqrkST98XKYz-epb4Wqyj-Y9zFB5Gw-BQwDo/edit#slide=id.gf596c35fb7_4_12


## UIs:
Factories live on metis, matic, rinkeby, mainnet. Will show up on switch to that chain
- Factory UIs
- Live site: https://factory.sharedtools.org
- Src: https://github.com/chimera-defi/factory-ui

- Vote escrow UI (live on mainnet)
- Live Site: https://sharedtools.org
- Src: https://github.com/chimera-defi/veToken-voting

## Dev tools:
- Hardhat-template
  https://github.com/chimera-defi/hardhat-template
- hardhat-framework
  https://github.com/chimera-defi/hardhat-framework
- smartcontract-UI
  https://github.com/chimera-defi/smartcontract-UI

## Contracts:
- Factory contracts  
https://github.com/chimera-defi/sharedtools-factory
- merkle-distributor-generic  
https://github.com/chimera-defi/merkle-distributor-generic
- Openzeppelin for OVM  
https://github.com/chimera-defi/openzeppelin-contracts-ovm

# Sponsor specific

## Matic
- Factories on Matic for Farming, vote Escrow, NFTs
- Viewable at https://factory.sharedtools.org
- Src: https://github.com/chimera-defi/factory-ui/commit/72978f4f8b42d8ec996740ae1f6c419c496b5fb8

## Metis
- Factories on metis for NFTs, Clones, VoteEscrow   https://github.com/chimera-defi/factory-ui/blob/master/utils/factories_metis.json
- Openzeppelin fork for OVM  
- Dev tooling to ease cross chain deploys at hardhat-template & hardhat-framework

## Rarible
- UI for Rarible ERCs live on rinkeby, mainnet
- MintableNFTSalesFactory for deploying custom NFTs e.g. for post-sale reveals of varied rarity NFTs, establishing minting caps and deadlines etc
  e.g. Src for ERC20 supporting MintableNFTSales https://github.com/chimera-defi/sharedtools-factory/blob/master/contracts/MintableNFTSaleERC20.sol
- NFT Merkle distributor for large audience NFT airdrops
  https://github.com/chimera-defi/merkle-distributor-generic/blob/master/contracts/ERC721MerkleDistributor.sol
  
## Uni
- UNI v3 position NFT to ERC20 mapper
- Allow using UNI v3 positions with old school masterchef/snx staking rewards contracts
- WIP - done as an attempt to dogfood dev tools
- SRC: https://github.com/chimera-defi/UniV3NFTERC20Mapper
- Deploy Rinkeby https://rinkeby.etherscan.io/address/0x706B8856e0e081c29e3Ba5c8bAA7D72D8E1d7CcC 
- Old deploy rinkeby with some manual testing https://rinkeby.etherscan.io/address/0x07f2a0cec0d3e15ef607cf7ac309057d38fad7a5#writeContract
- Also "improved" uni merkle distributors to support NFTs and ERC20 clawbacks and merkle root resets at https://github.com/chimera-defi/merkle-distributor-generic


## Yearn
- Weth vault strategy - wip - unsure of best way to proceed ala new vault or reuse old vault
https://github.com/chimera-defi/sharedstake-strategies/blob/master/contracts/vETH2CRVStrategy.sol

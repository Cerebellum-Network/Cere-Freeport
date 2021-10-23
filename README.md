# Freeport

## Mission statement

Today's NFT backed assets lack security and true ownership. The Cere Freeport (Decentralized Data Vault for NFT) is the first open and decentralized solution for this problem. 

This page provides a quick tutorial on the Freeport Creator Suite and a Quick Start Guide with documentation. It includes a set of Smart Contracts to deal with NFT (ERC1155) and auctions,
high-level services for Cere Decentralised Data Cloud (DDC) to store and retrieve assets and metadata, and a Creator Suite - front-end
application for NFT minting and asset uploads. 

## Tutorial

Connect your Wallet, Create NFTs and view created NFTs.

![Tutorial](https://user-images.githubusercontent.com/5919565/138561407-f5488c7b-e678-4292-8189-c7ab926d5734.gif)

## Modules overview

Building your own custom secure asset solutions for NFT's is challenging and very hard to decentralize. Cere Freeport is the all-in-one solution that helps you to launch NFT-backed features into your app much faster, all the features including minting NFT's, uploading NFT-based assets to Cere DDC (decentralized data cloud), configuring royalties, and even enabling permissioned NFT! The documentations below are the starting points (will be continously updated in the coming days):

|Name|Description|Status|Documentation|
|---|---|---|---|
|[Freeport Smart Contracts](https://github.com/Cerebellum-Network/Freeport-Smart-Contracts)|Set of Smart Contracts to to deal with NFT and auctions|Public (Apache 2.0 License)|[Readme](https://github.com/Cerebellum-Network/Freeport-Smart-Contracts/blob/master/README.md)|
|[Freeport S.C. Event Processor](https://github.com/Cerebellum-Network/Freeport-S.C.-Event-Processor)|Listens for events of Freeport Smart Contracts, calculates the state and stores it in DDC|Public (Apache 2.0 License)|[Readme](https://github.com/Cerebellum-Network/Freeport-S.C.-Event-Processor/blob/dev/README.md)|
|[Freeport DDC Gateway](https://github.com/Cerebellum-Network/Freeport-DDC-Gateway)|HTTP API for Freeport client applications|Private (soon public)|[Swagger](https://api.freeport.dev.cere.network/q/swagger-ui/)|
|[Freeport Media Service](https://github.com/Cerebellum-Network/Freeport-Media-Service)|High-level HTTP API to deal with assets in DDC|Private (soon public)|[Swagger](https://media.ddc.dev.cere.network/q/swagger-ui/)|
|[Freeport Creator Suite](https://github.com/Cerebellum-Network/Freeport-Creator-Suite)|UI for minting NFTs, upload assets and configure metadata|Private (soon public)||

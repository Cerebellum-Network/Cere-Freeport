# Freeport Quick Start Guide
## Introduction
Building your own custom secure asset solutions for NFTs is challenging and very hard to decentralize. Cere Freeport is the all-in-one solution that helps you to launch NFT-backed features into your app much faster, all the features including minting NFTs, uploading NFT-based assets to Cere DDC (Decentralized Data Cloud), configuring royalties, and even enabling permissioned NFT! Our team has all documentation you need prepared and ready to be used. This quick start guide provides you with an overview of how to use Freeport and integrate it with your app or game. With regards to integration there are even several options to choose from based on your preferred set-up. 
Freeport is currently an alpha release version. You can start using Freeport immediately. The Cere team will support with any technical challenges and will assist with enabling a data push/pull so you are all set to integrate your minted NFTs in your app or game. 

## Table of contents
* Who is this guide meant for
* High-level steps
* Minimal requirements
* How to use Freeport
* How to integrate the Cere SDK in your app or game
* Modules overview

## Who is this guide meant for
This repo aims to be beneficial to applications & developers who are looking to easily build value-adding NFT experiences in their application or game. 

## Minimal requirements
Current stage (alpha preview)

* Web3 wallet (e. g. Metamask) with Matic/Polygon tokens.

In future
* Polkadot-compatible wallet with Cere tokens for DDC usage

Custom set-up (upon request)
* Web3 wallet for any Ethereum-compatible network
* Polkadot-compatible wallet with Cere tokens for DDC usage


## High-level steps
1. Use the Freeport Creator Suite to mint the NFTs
2. Integrate the Cere SDK in your app/game (SDK documentation)
3. Distribute NFTs to users everywhere (in-game & marketplaces)
4. Receive partner grants in $CERE based on activity milestones reached

## How to use Freeport
Use the Freeport Creator Suite to mint your NFTs and securely add data relevant for your use case. The following steps explain you how to create NFTs with Freeport:
1. Go to [Freeport](https://davinci.stage.cere.network)  
2. Connect your wallet
3. Mint NFTs (smart contract call from UI)
4. Configure NFTs (pricing, royalties, auction etc.)
5. Upload data/assets to Cere DDC(smart contract call from UI)

Note: DDC usage is currently free of charge

## How to connect Freeport to your app or game
With regards to integration there are even several options to choose from based on your preferred set-up. The Cere team will support with any technical challenges and will assist with enabling a data push/pull so you are all set to integrate your minted NFTs in your app or game. 

A high-level overview for connecting Freeport with help of the Cere SDK to other software:
1. Push model (link to push model)
* Basic Freeport CMS or your own CMS (link to CMS integration)
* Backend Services (link to backend services integration)
2. Pull model (link to pull model)
3. Advanced options (upon request)

### Push model
Freeport NFT (related) data can be pushed to your application or game however you like. Freeport provide multiple ways for you to do so. Data can be pushed to a CMS that can connect to your application or game. You have the option to use the basic CMS provided by Freeport or your own CMS. In case you have any backend services Freeport can push data directly to you.

**Option 1: CMS**
1. Set-up CMS with basic Freeport set-up or your own
2. Configure CMS for your application: create entities, content templates
3. Send us your CMS configuration: URL, authentication token
4. (We will add this inside Freeport)
5. Data from Freeport is sent to CMS (Sergey currently working on)

**Option 2: Backend Services**
1. Configure back-end service to accept POST and PUT requests from Freeport
2. Configure data model to match Freeport model (you can also process requests manually)
3. Configure access token for Freeport
4. Register your application URL with help of Cere team and access token

### Pull model
Freeport provides a high-level API and low level tools for custom integrations with which you can pull data into your application or game. The steps are straight forward:
1. Simply make your request for needed data
2. Retrieve data from Freeport 

### Advanced options
If the above options do not work for your app or game, or you prefer another route there is some alternatives routes that can be set-up upon request.

* Integration with message queues (Kafka, SQS or similar)
* Direct access to DB for CDC (capture data changes)

## Customization options

**Freeport services in isolated environment** 

* Smart Contracts
* Creator Suite
* DDC Proxy
* Events listener and processor
* CMS
* Private DDC Cluster

**Additional services for application needs**

* Integration with CDN providers
* CMS configuration
* Development and architectural support


## Modules overview
The documentations below are the starting points (will be continuously updated along the way):

|Name|Description|Status|Documentation|
|---|---|---|---|
|[Freeport Smart Contracts](https://github.com/Cerebellum-Network/Freeport-Smart-Contracts)|Set of Smart Contracts to to deal with NFT and auctions|Public (Apache 2.0 License)|[Readme](https://github.com/Cerebellum-Network/Freeport-Smart-Contracts/blob/master/README.md)|
|[Freeport Smart Contracts SDK](https://github.com/Cerebellum-Network/Freeport-Smart-Contracts-SDK)|The JavaScript SDK of Freeport|Public (Apache 2.0 License)|[Readme](https://github.com/Cerebellum-Network/Freeport-Smart-Contracts-SDK/blob/master/README.md)|
|[Freeport S.C. Event Processor](https://github.com/Cerebellum-Network/Freeport-S.C.-Event-Processor)|Listens for events of Freeport Smart Contracts, calculates the state and stores it in DDC|Public (Apache 2.0 License)|[Readme](https://github.com/Cerebellum-Network/Freeport-S.C.-Event-Processor/blob/dev/README.md)|
|[Freeport Creator Suite](https://github.com/Cerebellum-Network/Freeport-Creator-Suite)|UI for minting NFTs, upload assets and configure metadata|Private (soon public)||
|[Freeport Media Service](https://github.com/Cerebellum-Network/Freeport-Media-Service)|High-level HTTP API to deal with assets in DDC|Private (soon public)|[Swagger](https://media.ddc.dev.cere.network/q/swagger-ui/)|
|[Freeport DDC Gateway](https://github.com/Cerebellum-Network/Freeport-DDC-Gateway)|HTTP API for Freeport client applications|Private (soon public)||

We’re here to help with. Freeport is currently an alpha release version. You can start using Freeport immediately. The Cere team will support with any technical challenges and will assist with enabling a data push/pull so you are all set to integrate your minted NFTs in your app or game. Do not hestitate to reach out.

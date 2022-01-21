# Freeport

## Mission statement

Today's NFT backed assets lack security and true ownership. The Cere Freeport (Decentralized Data Vault for NFT) is the first open and decentralized solution for this problem. 

This page provides a quick tutorial on the Freeport Creator Suite and a Quick Start Guide with documentation. It includes a set of Smart Contracts to deal with NFT (ERC1155) and auctions,
high-level services for Cere Decentralised Data Cloud (DDC) to store and retrieve assets and metadata, and a Creator Suite - front-end
application for NFT minting and asset uploads. 

## Tutorial

Connect your Wallet, Create NFTs and view created NFTs.

![Tutorial](https://user-images.githubusercontent.com/5919565/138561407-f5488c7b-e678-4292-8189-c7ab926d5734.gif)

## Quick Start Guide

Building your own custom secure asset solutions for NFTs is challenging and very hard to decentralize. Cere Freeport is the all-in-one solution that helps you to launch NFT-backed features into your app much faster, all the features including minting NFTs, uploading NFT-based assets to Cere DDC (Decentralized Data Cloud), configuring royalties, and even enabling permissioned NFT! 
Our team has all documentation you need prepared and ready to be used. The [Quick Start Guide](https://github.com/Cerebellum-Network/Cere-Freeport/blob/3135c31270ae200c38b8f374af30c35583268f4a/Quick-Start-Guide.md) provides you with an overview of how to use Freeport and integrate it with your app or game. Freeport is currently an alpha release version. You can start using Freeport immediately. The Cere team will support with any technical challenges and will assist with enabling a data push/pull so you are all set to integrate your minted NFTs in your app or game. Integrate and start using Freeport right now with help of our [Quick Start Guide](https://github.com/Cerebellum-Network/Cere-Freeport/blob/3135c31270ae200c38b8f374af30c35583268f4a/Quick-Start-Guide.md). 

## Modules overview

The documentations below are the starting points (will be continuously updated along the way):

|Name|Description|Status|Documentation|
|---|---|---|---|
|[Freeport Smart Contracts](https://github.com/Cerebellum-Network/Freeport-Smart-Contracts)|Set of Smart Contracts to to deal with NFT and auctions|Public (Apache 2.0 License)|[Readme](https://github.com/Cerebellum-Network/Freeport-Smart-Contracts/blob/master/README.md)|
|[Freeport Smart Contracts SDK](https://github.com/Cerebellum-Network/Freeport-Smart-Contracts-SDK)|The JavaScript SDK of Freeport|Public (Apache 2.0 License)|[Readme](https://github.com/Cerebellum-Network/Freeport-Smart-Contracts-SDK/blob/master/README.md)|
|[Freeport S.C. Event Processor](https://github.com/Cerebellum-Network/Freeport-S.C.-Event-Processor)|Listens for events of Freeport Smart Contracts, calculates the state and stores it in DDC|Public (Apache 2.0 License)|[Readme](https://github.com/Cerebellum-Network/Freeport-S.C.-Event-Processor/blob/dev/README.md)|
|[Freeport Creator Suite](https://github.com/Cerebellum-Network/Freeport-Creator-Suite)|UI for minting NFTs, upload assets and configure metadata|Private (soon public)||
|[Freeport DDC Proxy](https://github.com/Cerebellum-Network/Freeport-Media-Service)|High-level HTTP API to deal with assets in DDC|Private (soon public)|[Swagger](https://media.ddc.dev.cere.network/q/swagger-ui/)|
|[Freeport API](https://github.com/Cerebellum-Network/Freeport-DDC-Gateway)|HTTP API for Freeport client applications|Private (soon public)||

We’re here to help with. Freeport is currently an alpha release version. You can start using Freeport immediately. The Cere team will support with any technical challenges and will assist with enabling a data push/pull so you are all set to integrate your minted NFTs in your app or game. Do not hestitate to reach out.

## Run all services with Docker Compose

1. Create your own API key in [Covalent](https://www.covalenthq.com).
2. Navigate to `docker-compose/` directory `cd docker-compose/`.
3. Put your API key in the `.env` file.
4. Run `docker-compose -f docker-compose-all-dev.yaml up -d` to start all services.

The following services will be exposed:

- Freeport API at port 8080 (http://localhost:8080/q/swagger-ui)
- Freeport DDC proxy at port 8081 (http://localhost:8081/q/swagger-ui)
- DDC Cluster with 3 nodes at ports 8888, 8881, 8882
- S3 service at port 9000 (region: `us-east-1`, access key id: `test-key`, secret access key: `test-secret`)
- PostgreSQL at port 5432 (user: `pg`, password: `pwd`, database: `freeport`)

Test DDC keys:
- Public: `0xdab1b135fbeb366b9a3a2e63d6e05152998dd3046cd91344a615f5ed82c2b431`
- Private: `0xd840107172a79d69287e424a4c2a4f673e59a0510948e37a3a1c9458da4b9371`

Current version of the Docker compose file is pointed to development environment and uses smart contracts from Polygon Mumbai Testnet.
You might need to wait some time until data from chain will be synchronized with local database.

# Origin
Origin is a set of toolkits that together provide a system for issuance and management of Energy Attribute Certificates (EACs). This repository is an entry point to Origin systems. It has a goal of explaining briefly the whole system and providing you with insight and info where to explore next. 

## Table of Contents
- [Energy Attribute Certificates](#energy-attribute-certificates)
- [How does it work](#how-does-it-work)
- [Key modules and components](#key-modules-and-components)
- [Where to start](#where-to-start)
- [Deployment](#deployment)

## Energy Attribute Certificates
Energy Attribute Certificates, or EACs, is an official document which guarantees that produced energy comes from a renewable source. There are different standards that regulate how data is stored and validated. In Europe, this document is called Guarantee of Origin (GO), in North America, it's called Renewable Energy Certificate (REC), and in parts of Asia, Africa, the Middle East, and Latin America governing standard is International REC (I-REC). Standards do vary, but they all share the same core principles. 

The main purpose of EACs is to act as an accounting vehicle to prove that consumed energy came from a renewable source. EACs are mostly used to address sustainability reports regarding [Scope 2 emissions](https://en.wikipedia.org/wiki/Carbon_emissions_reporting#Scope_2:_Electricity_indirect_GHG_emissions).

## How does it work
_Brief description of how it works from reading data in the real world to trading and retiring certificates. Links to learn more_

## Key modules and components
Overview of architecture

### Key repositories

This section lists key entry points to start your journey with Origin. 

1. [ew-utils-demo](https://github.com/energywebfoundation/ew-utils-demo) - demo repository with build scripts that enable easy deployment of smart contracts to Tobalaba or local blockchain. Often used to demo and get to know features and capabilities of Origin. 
2. [ew-utils-testbackend](https://github.com/energywebfoundation/ew-utils-testbackend) - Origin combines on and off-chain data storage. This repository is used to act as a backend service for off-chain data storage. You'll need this to run `ew-utils-demo` (store data), and `ew-origin-ui` to display stored data. 
3. [ew-origin-ui](https://github.com/energywebfoundation/ew-origin-ui) - frontend of the system needed to view data stored in smart contracts (on-chain) and in the backend (off-chain). To interact Origin frontend you'll need [MetaMask](https://metamask.io).

### Other components

1. [ew-user-registry-lib](https://github.com/energywebfoundation/ew-user-registry-lib) - high-level library to interact with user registry. Can be used to i. a. create new user or set user's role in the system.
2. [ew-asset-registry-lib](https://github.com/energywebfoundation/ew-asset-registry-lib) - high-level library for creating and managing electricity producing and consuming assets. Depends on [ew-user-registry-lib](https://github.com/energywebfoundation/ew-user-registry-lib), because only user with Asset Manager role can be owner of asset. 
3. [ew-origin-lib](https://github.com/energywebfoundation/ew-origin-lib) - a heart of Origin systems, contains logic for storing and transferring Energy Attribute Certificates (as a form of unique [ERC721](http://erc721.org/) tokens). This library also has a more general construct called **TradeableEntity** that can be used to wrap, as name suggests, other tradeable entities, such as [Power Purchase Agreements](https://en.wikipedia.org/wiki/Power_purchase_agreement) or certificate bundles.
4. [ew-market-lib](https://github.com/energywebfoundation/ew-market-lib/) - a library that allows to create demand (for buyers), supply (for sellers) and agreements between buyers and sellers.
5. [ew-market-matcher](https://github.com/energywebfoundation/ew-market-matcher) - the most important part of marketplace, guarantees automatic matching of supply and demand between sellers and buyers. Matching rules can be highly customized and afterwards the algorithm can be tested by running matching simulator.
6. [ew-erc-test-contracts](https://github.com/energywebfoundation/ew-erc-test-contracts) - Test ERC20 token for demo purposes, especially for doing an on-chain test purchase of a certificate using tokens
7. [ew-utils-general-lib](https://github.com/energywebfoundation/ew-utils-general-lib) - Contains logic for more straightforward interaction with contracts, such as watching events. It is also a base layer for other libraries to build upon. It provides a foundation for things like off-chain data storage that is universal for all entities.

## Where to start
_Explain where our demo is and what's the purpose of running a demo. Identify Origin team and ways how to connect with them_

## Deployment

For deployment instructions please refer to [Docker Deployment](https://github.com/energywebfoundation/origin/wiki/Docker-Deployment) wiki page.
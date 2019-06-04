# Origin
Origin is a set of toolkits that together provide a system for issuance and management of Energy Attribute Certificates (EACs). This repository is an entry point to Origin systems. It has a goal of explaining briefly the whole system and providing you with insight and info where to explore next. 

## Table of Contents
- [Energy Attribute Certificates](#energy-attribute-certificates)
- [How does it work](#how-does-it-work)
- [Key modules and components](#key-modules-and-components)
- [Where to start](#where-to-start)

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

1. [ew-user-registry-lib](https://github.com/energywebfoundation/ew-user-registry-lib) - User registry and role management logic
2. [ew-asset-registry-lib](https://github.com/energywebfoundation/ew-asset-registry-lib) - Consuming assets/Producing assets registry
3. [ew-origin-lib](https://github.com/energywebfoundation/ew-origin-lib) - Contains Certificate and TradeableEntity logic, including registry of Certificate ownership
4. [ew-market-lib](https://github.com/energywebfoundation/ew-market-lib/) - Market logic and contracts, including Demand storage
5. [ew-market-matcher](https://github.com/energywebfoundation/ew-market-matcher) - Supply and Demand matching logic
6. [ew-erc-test-contracts](https://github.com/energywebfoundation/ew-erc-test-contracts) - Test ERC token for demo purposes
7. [ew-utils-general-lib](https://github.com/energywebfoundation/ew-utils-general-lib) - Contains logic for more straightforward interaction with contracts, such as watching events


## Where to start
_Explain where our demo is and what's the purpose of running a demo. Identify Origin team and ways how to connect with them_

# Origin
_Brief description of what Origin is (3-5 sentences)_

## Table of Contents
- [Certificates of Origin](#certificates-of-origin)
- [How does it work](#how-does-it-work)
- [Key modules and components](#key-modules-and-components)
- [Where to start](#where-to-start)

## Certificates of Origin
_Brief description and links to learn more_

## How does it work
_Brief description of how it works from reading data in the real world to trading and retiring certificates. Links to learn more_

## Key modules and components
Overview of architecture

### Key repositories

This section lists key entry points to start your journey with Origin. 

1. [ew-utils-demo](https://github.com/energywebfoundation/ew-utils-demo) - use to deploy contracts to Tobalaba or local blockchain
2. [ew-utils-testbackend](https://github.com/energywebfoundation/ew-utils-testbackend) - needed for `ew-utils-demo` to store off-chain data and later for frontend to retrieve it
3. [ew-origin-ui](https://github.com/energywebfoundation/ew-origin-ui) - React frontend to interact with Origin deployment through browser and MetaMask

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

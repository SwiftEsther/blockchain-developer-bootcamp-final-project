# NFT
A contract that allows users mint and burn Non-fungible Token. It allows users to create a mintable/burnable NFT collection

## Demo
https://mih-nft-ui.herokuapp.com/
https://www.loom.com/share/ec9d93239cd148288567a310640fcca2

## Directory structure

```
.
├── contracts/              // Solidity smart contracts
├── docs/
│   ├── avoiding_common_attacks.md
│   └── design_pattern_decisions.md
├── frontend/               // Web app
├── test/                   // Mocha + Chai contract tests
├── deployed_addresses.txt  // Contract addresses on Rinkeby
├── README.md               // You are here!
├── ...
```

## NFT recipient account address

`0x...`

# Usage

## Install dependencies

*Prerequisite: You must have node.js and npm installed*

```sh
npm install -g truffle
npm install @openzeppelin/contracts
npm i -g --only=prod https-localhost # Only if running the app locally
```

## Accessing the project
<!-- link to frontend -->

## Running locally

*Prerequisite: You must run a local blockchain like Ganache in the background*

```sh
truffle compile
truffle migrate
cd frontend/
serve . # May need sudo depending on OS
```

Open `localhost`, switch Metamask to your local blockchain network, and connect

### Create a frontend/env.js file containing the following

```
const INFURA_PROJECT_ID=<insert_yours_here>
const CONTRACT_ADDRESS_RINKEBY=<from_truffle_migrate>
const CONTRACT_ADDRESS_LOCAL=<from_ganache>
```

## Run unit tests

```sh
truffle test
```


## Possible issues
`Error: ENOENT: no such file or directory, open '.secret'`
Solution: You'll need a mnemonic - the twelve word phrase the wallet uses to generate public/private key pairs

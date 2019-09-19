# Dapp on Ethereum for CryptoStar

<img width="1131" alt="etherscan" src="https://raw.githubusercontent.com/osamabari/Dapp_notary_app/master/image/etherscan.png">

## Token Info

* ERC-721 token name : "Star Token"

* ERC-721 token symbol : "STR"

* Contract Address in Rinkeby Network : 0x929248153a771425EbAf0D6d3F0130Dd5fB91472

  ```
     Replacing 'StarNotary'
     ----------------------
  > block number:        5115793
   > block timestamp:     1568875665
   > account:             0xCf6061886e9aB888fBB3267eE501970D476FB6C4
   > balance:             0.0695575
   > gas used:            2667934
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.02667934 ETH
   > Total cost:          0.02667934 ETH
  ```

  

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

To install the software, you need to doownload the following:

1. Install [Node.js](https://nodejs.org/en/) on your computer.
2. Clone or download the repository to your local computer.
3. Open the terminal and install the packages: `npm install` or `yarn`

If you want deploy the smart contract to Rinkeby network, you need to the following:

1. The Metamask's backup phrase is required.
2. [Infura](https://infura.io/) Project ID

### Installing

The procedure to obtain development environment:

```
npm install --save truffle-hdwallet-provider
npm install --save openzeppelin-solidity
```

Run the truffle develope. *Truffle Develop started at http://127.0.0.1:9545/*

And You can get Accounts and Private Keys.

```
truffle develope
```

You have to type following command on New Terminal and Deploy the smart contract on the your rinkbey.

```
truffle migrate --network rinkeby --reset --compile-all
```



To run the front-end of the Dapp, You have to type following command on New Terminal.

```
cd app
```

Start the webpack-dev-server  *Project is running at http://localhost:8080/*

```
npm run dev
```

Open that url in your browser to access the front-end of the Dapp.



### Deploy the Smart Contract to Rinkeby Network

If you want deploy the smart contract to Rinkeby network, you need to the following:

* You have to type your infura Project ID to `const infuraKey = {Infura POJECT ID}` in truffle-config.js file.
* Type Metamask's backup phrase to `const mnemonic = {METAMASK SEED}` in truffle-config.js file.
* Type `truffle migrate --network rinkeby --reset --compile-all` on the terminal.



## Running the tests

Explain how to run the automated tests for this system.

* You can run the unit test smart contract by `test` command on truffle console.

```
truffle(develop)> test
Using network 'develop'.


Compiling your contracts...
===========================
> Everything is up to date, there is nothing to compile.



Compiling your contracts...
===========================
> Everything is up to date, there is nothing to compile.



  ✓ can create a Star (75ms)
  ✓ lets user1 put up their star for sale (103ms)
  ✓ lets user1 get the funds after the sale (164ms)
  ✓ lets user2 buy a star, if it is put up for sale (169ms)
  ✓ lets user2 buy a star and decreases its balance in ether (135ms)
  ✓ can add the star name and star symbol properly (68ms)
  ✓ lets 2 users exchange stars (139ms)
  ✓ lets a user transfer a star (90ms)
  ✓ lookUptokenIdToStarInfo test (73ms)

  9 passing (1s)
```



## Built With

* [Node.js](https://nodejs.org/en/) v11.9.0 - The JavaScript used.
* [Truffle](https://truffleframework.com/) v5.0.26 - A development framework for Ethereum.
* [openzeppelin-solidity]() v2.3.0 - Library for secure smart contract development.

## Author

* **Osama Bari** - [Github](https://github.com/osamabari)

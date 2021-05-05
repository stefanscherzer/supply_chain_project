# Udacity Blockchain Developer ND
## PROJECT: Supply Chain

<br>

For this project, I created a DApp by adding functionality to a prepared smart contract
([project](https://github.com/udacity/nd1309-Project-6b-Example-Template))
and deployed it on the public Rinkeby testnet.

<br>

Description by Udacity:  
> This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

<br>

I used the following versions to run the project:  

Ganache CLI v6.12.2 (ganache-core: 2.13.2)  
Truffle v5.3.2 (core: 5.3.2)  
Solidity v0.5.16 (solc-js)  
Node v15.14.0  
Web3.js v1.3.5

<br>

E.g., [Contract](https://rinkeby.etherscan.io/address/0x66020930e8708761cfa11a0b9c2d68bfb87e816c)
on the Rinkeby Network

<br>

---

<br>

## Project write-up
### UML


### Libraries


### IPFS

<br>

---

<br>

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

<br>

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

Here is how you check which ganache-cli and Truffle version you have installed:

```
ganache-cli --version   

Ganache CLI v6.12.2 (ganache-core: 2.13.2)
```                                                                           

```
truffle version

Truffle v5.3.2 (core: 5.3.2)  
Solidity v0.5.16 (solc-js)  
Node v15.14.0  
Web3.js v1.3.5
```

If you need to install one of the mentioned tools, follow the How-tos mentioned here:

- [How to install ganache-cli](https://github.com/trufflesuite/ganache-cli#installation)
- [How to install truffle](https://www.trufflesuite.com/truffle)
- [How to install Metamask](https://metamask.io/download.html)

<br>

### Installing

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/stefanscherzer/supply_chain_project.git
```

Install all requisite npm packages (as listed in ```package.json```):

```
npm install
```

Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

Your terminal should look something like this:

![ganache-cli](images/ganache-cli.png)

---

In a separate terminal window, Compile your smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle compile](images/truffle_compile.png)

This will create the smart contract artifacts in folder ```build\contracts```.

---

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle migrate I](images/truffle_migrate1.png)  

![truffle migrate II](images/truffle_migrate2.png)  

![truffle migrate III](images/truffle_migrate3.png)

---

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

---

In a separate terminal window, launch the DApp:

```
npm run dev
```


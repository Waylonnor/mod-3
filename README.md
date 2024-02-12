# CustomToken Contract

## Introduction

This repository contains a Solidity smart contract for a custom ERC20 token called CustomToken. The contract allows for the creation of a new ERC20 token with custom parameters, such as token name, symbol, initial supply, and owner. It also includes functions for minting, burning, and transferring tokens.

## Contract Overview

### ERC20 Functionality

The CustomToken contract inherits from the ERC20 standard, which is an interface for implementing ERC20 tokens on the Ethereum blockchain. This means that the CustomToken contract supports all standard ERC20 functions, such as `balanceOf`, `transfer`, `approve`, `allowance`, and `transferFrom`.

### Ownable

The CustomToken contract also inherits from the Ownable contract provided by OpenZeppelin. This adds functionality for ownership control, allowing certain functions to be restricted to only the owner of the contract.

### Constructor

The constructor function is used to initialize the CustomToken contract with initial parameters. These parameters include the token name, symbol, initial supply, and the address of the initial owner of the tokens.

### Custom Functions

1. **mintTokens**: This function allows the owner of the contract to mint new tokens and distribute them to a specified recipient.

2. **burnTokens**: This function allows any token holder to burn a specified amount of their tokens, effectively removing them from circulation.

3. **transferTokens**: This function allows token holders to transfer tokens to another address.

## Getting Started

To deploy and interact with the CustomToken contract, you will need the following:

1. An Ethereum development environment (e.g., Remix, Truffle, Hardhat).
2. Access to an Ethereum wallet (e.g., MetaMask) connected to the desired network (e.g., Ethereum mainnet, Ropsten testnet).
3. The Solidity source code for the CustomToken contract.

## Deployment

To deploy the CustomToken contract, follow these steps:

1. Compile the Solidity code using your preferred development environment.
2. Deploy the compiled contract to the desired Ethereum network using a deployment script or tool.
3. Provide the necessary constructor arguments (token name, symbol, initial supply, initial owner address) during deployment.

## Interacting with the Contract

Once deployed, you can interact with the CustomToken contract using various Ethereum wallet interfaces or through custom dApps. Use the following methods to interact with the contract:

- **Minting Tokens**: Call the `mintTokens` function with the desired recipient address and token amount. Only the contract owner can mint tokens.

- **Burning Tokens**: Call the `burnTokens` function with the desired amount of tokens to burn. Any token holder can burn their own tokens.

- **Transferring Tokens**: Call the `transferTokens` function to transfer tokens from one address to another.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Author

Waylon

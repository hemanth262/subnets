# Solidity Smart Contracts 

This repository contains two Solidity smart contracts: `Vault` and `ERC20`. Each contract serves a distinct purpose and showcases various features of the Ethereum blockchain. Below, you will find an overview of each contract and instructions on how to deploy and interact with them.

## 1. Vault Smart Contract

### Overview

The `Vault` smart contract is designed to manage deposits and withdrawals of ERC-20 tokens. It utilizes the `IERC20` interface for interaction with ERC-20 tokens and implements functions for depositing and withdrawing tokens based on a share system.

### Functions

1. **deposit(uint _amount):**
   - Allows users to deposit ERC-20 tokens into the vault.
   - Calculates the number of shares to mint based on the current total supply and token balance.

2. **withdraw(uint _shares):**
   - Enables users to withdraw ERC-20 tokens from the vault by burning a specific number of shares.
   - Calculates the amount of tokens to be withdrawn based on the user's shares and the current total supply.

### Deployment

1. Deploy the `Vault` smart contract, passing the address of the desired ERC-20 token as a constructor argument.

2. Users can interact with the contract by depositing and withdrawing tokens using the provided functions.

## 2. ERC20 Token Smart Contract

### Overview

The `ERC20` smart contract is a basic implementation of the ERC-20 token standard. It includes functionalities for transferring tokens, approving spending, and managing allowances. The contract also allows for minting and burning tokens, showcasing the flexibility of ERC-20 tokens.

### Functions

1. **transfer(address recipient, uint amount):**
   - Transfers a specified amount of tokens from the sender's balance to the recipient.

2. **approve(address spender, uint amount):**
   - Approves a spender to withdraw a specified amount of tokens from the sender's account.

3. **transferFrom(address sender, address recipient, uint amount):**
   - Transfers a specified amount of tokens from the sender to the recipient if the sender has sufficient allowance.

4. **mint(uint amount):**
   - Mints a specified amount of new tokens and adds them to the total supply.

5. **burn(uint amount):**
   - Burns a specified amount of tokens, reducing the total supply.

### Deployment

1. Deploy the `ERC20` smart contract, providing details such as name, symbol, and decimals.

2. Users can interact with the contract by transferring tokens, approving spending, minting new tokens, and burning existing tokens.

## License

Both smart contracts are released under the MIT License. See the `LICENSE` file for details.


## Author

Hemanth N

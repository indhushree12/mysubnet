# Vault Contract and ERC20 Token Contract

This repository contains two Solidity contracts: `Vault` and `ERC20`.

## Vault Contract

The `Vault` contract is designed to manage deposits and withdrawals of ERC20 tokens. Key functionalities include:

- **Deposit:** Users can deposit ERC20 tokens into the vault contract. Upon deposit, the tokens are converted into shares, with the number of shares proportional to the deposited amount relative to the total supply of tokens in the vault.
- **Withdraw:** Users can withdraw tokens from the vault, receiving back an equivalent amount based on their share ownership in the vault.

### Functions:

- `deposit(uint _amount) external`: Allows users to deposit ERC20 tokens into the vault.
- `withdraw(uint _shares) external`: Allows users to withdraw ERC20 tokens from the vault.

### Variables:

- `totalSupply`: Total number of shares in the vault.
- `balanceOf`: Mapping of user addresses to their respective share balances.

## ERC20 Contract

The `ERC20` contract is a standard implementation of the ERC20 token. It provides basic functionalities for transferring tokens, managing allowances, and minting/burning tokens.

### Functions:

- `transfer(address recipient, uint amount) external`: Transfers tokens from the sender's address to the recipient's address.
- `approve(address spender, uint amount) external`: Approves a spender to spend a certain amount of tokens on behalf of the owner.
- `transferFrom(address sender, address recipient, uint amount) external`: Transfers tokens from one address to another, with allowance validation.
- `mint(uint amount) external`: Mints new tokens and assigns them to the sender's address.
- `burn(uint amount) external`: Burns tokens from the sender's address, reducing the total token supply.

### Variables:

- `totalSupply`: Total supply of the ERC20 token.
- `balanceOf`: Mapping of addresses to their respective token balances.
- `allowance`: Mapping of owner addresses to spender addresses and the amount of tokens approved for spending.

## Author

indhushree 

indushree736@gmail.com


## License

Both contracts are provided under the MIT License. Please refer to the SPDX-License-Identifier tags within the contracts for more details.

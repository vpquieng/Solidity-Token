# MyToken Smart Contract

## Overview

**MyToken** simple ERC20-like token implemented in Solidity. It allows users to mint and burn tokens, while tracking the total supply and user balances. This contract is built on Ethereum's Solidity version `0.8.26`.

## Features

- Public token details such as **Token Name**, **Token Abbreviation**, and **Total Supply**.
- A mapping of Ethereum addresses to balances.
- Minting function to create new tokens.
- Burning function to destroy tokens.
- Safeguards to ensure tokens can only be burned if the address has a sufficient balance.

## Contract Details

- **Token Name**: `SolidCoin`
- **Token Abbreviation**: `SLC`
- **Solidity Version**: `0.8.26`

### Functions

#### 1. mint(address _to, uint256 _amount)
The `mint` function allows for the creation of new tokens. It increases the total supply and adds the minted tokens to the balance of the specified address.

```solidity
function mint(address _to, uint256 _amount) public;
```

#### 2. burn(address _from, uint256 _amount)
The 'burn' function destroys tokens. It decreases the total supply and reduces the balance of the specified address. It ensures that an address has sufficient tokens before burning them.

```solidity
function burn(address _from, uint256 _amount) public;
```

### Requirements
To use this contract, you need:

- Solidity Compiler: Version 0.8.26 or higher.
- Ethereum Development Environment: Such as Remix, Hardhat, or Truffle.

### How to use

1. Clone the repository to your local machine:

```solidity
git clone https://github.com/your-username/mytoken-contract.git
cd mytoken-contract
```

2. Deploy the Contract: Use any Ethereum development environment or Remix IDE to deploy the contract.

3. Mint Tokens: Call the mint function to create new tokens for a specific address.

4. Burn Tokens: Use the burn function to destroy tokens from an address, ensuring the address has enough tokens to burn.

### Example
Here's an example of how to interact with the contract:

- Mint 100 tokens:
```solidity
mint(address(0xRecipientAddress), 100);
```
- Burn 50 tokens
## Contributors
```solidity
burn(address(0xHolderAddress), 50);
```
- **Vincent Paul Quieng** - Developer 

## License 

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.


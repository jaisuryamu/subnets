**README.md**

# ERC20 Token and Vault Contract

## Overview

This repository contains the implementation of an ERC20 token contract and a Vault contract. The ERC20 token contract defines a standard interface for fungible tokens on the Ethereum blockchain, while the Vault contract provides a secure way to store and manage these tokens.

## ERC20 Token Contract

The ERC20 token contract implements the standard functions and events defined by the ERC20 token standard. It allows for the creation and management of fungible tokens on the Ethereum blockchain. Users can transfer tokens to other addresses, approve spending limits for other addresses, and check token balances. The contract also emits events for token transfers and approvals.

### ERC20 Functions

- `totalSupply()`: Returns the total supply of tokens.
- `balanceOf(address account)`: Returns the token balance of the specified address.
- `transfer(address to, uint256 amount)`: Transfers tokens from the sender's address to the specified recipient.
- `transferFrom(address from, address to, uint256 amount)`: Transfers tokens on behalf of another address (requires approval).
- `approve(address spender, uint256 amount)`: Approves the specified address to spend the sender's tokens.
- `allowance(address owner, address spender)`: Returns the amount of tokens approved for spending by a specific address.
  
### ERC20 Events

- `Transfer(address indexed from, address indexed to, uint256 value)`: Emitted when tokens are transferred from one address to another.
- `Approval(address indexed owner, address indexed spender, uint256 value)`: Emitted when an approval for token spending is granted.

## Vault Contract

The Vault contract provides a secure way to store and manage ERC20 tokens. It allows users to deposit and withdraw tokens into/from the vault. Additionally, the vault owner can transfer tokens from the vault to other addresses.

### Vault Functions

- `deposit(uint256 amount)`: Allows users to deposit tokens into the vault.
- `withdraw(uint256 amount)`: Allows users to withdraw tokens from the vault.
- `transfer(address to, uint256 amount)`: Allows the vault owner to transfer tokens from the vault to another address.
- `tokenBalance()`: Returns the balance of ERC20 tokens held in the vault.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

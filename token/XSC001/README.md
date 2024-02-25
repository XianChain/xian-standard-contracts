# XSC001 Token Contract

The `XSC001` token contract is a standardized smart contract developed for the Xian blockchain. This contract implements a basic token system with functionalities such as token transfer, approval mechanisms, and metadata management. It is designed to serve as a foundational component for building decentralized applications on the Xian network.

## Contract Overview

The `XSC001` contract includes mechanisms for:

- Initial token distribution
- Metadata management
- Token transfers
- Approval and transfer from approved accounts

## Functions

### `@construct def seed()`

This function is called upon contract creation and initializes the contract's state. It sets the initial token balance for the creator and establishes basic token metadata such as the token name, symbol, logo URL, website, and operator.

**Parameters:**
- None

### `@export def change_metadata(key: str, value: Any)`

Allows the operator to update the metadata of the token.

**Parameters:**
- `key`: The metadata key to update (e.g., 'token_name', 'token_symbol').
- `value`: The new value for the specified key.

### `@export def transfer(amount: float, to: str)`

Enables token holders to transfer tokens to another account.

**Parameters:**
- `amount`: The amount of tokens to be transferred.
- `to`: The recipient's address.

### `@export def approve(amount: float, to: str)`

Allows a token holder to approve another account to spend a specified amount of tokens on their behalf.

**Parameters:**
- `amount`: The amount of tokens to be approved.
- `to`: The address of the account that is being approved to spend tokens.

### `@export def transfer_from(amount: float, to: str, main_account: str)`

Enables an approved account to transfer tokens on behalf of the token holder.

**Parameters:**
- `amount`: The amount of tokens to transfer.
- `to`: The recipient's address.
- `main_account`: The address of the token holder who has approved the sender to spend tokens on their behalf.


## Contact

For further assistance or to report issues, please open an issue in the main repository or contact the project maintainers directly.

Thank you for your interest in the `XSC001` token contract for the Xian blockchain.

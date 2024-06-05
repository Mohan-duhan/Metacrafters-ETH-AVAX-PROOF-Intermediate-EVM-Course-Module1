# Solidity Contract Readme

📄 **Assessment.sol** - A Simple Solidity Contract for Managing Balances

This is a simple Solidity contract designed for managing balances with error handling using `require` statements and demonstrating the use of modifiers.

## Contract Overview

The `Assessment` contract includes the following functionality:

- A public variable `currBalance` that represents the current balance of the contract.
- A public variable `author` that stores the address of the contract creator.
- Modifiers for access control and balance checks.
- Functions to deposit and withdraw funds.

## ⚠️ Error Handling

### `require()`

The `require()` statement is used to validate certain conditions before further execution of a function. If the condition is not met, the execution is reverted with an optional error message.

require(<condition to be validated>, <message to be displayed if the condition fails>);

### `assert()`
The `assert()` statement is used to check for conditions that should always be true. If the condition fails, the execution is terminated with an error message, and it generally indicates a bug in the contract.

assert(<condition to be checked/validated>);


### `revert()`
The `revert()` statement can be used to flag an error and revert the current call. It can include a message providing details about the error, which will be passed back to the caller.

revert(<message providing details about the error>);


By employing these error handling mechanisms effectively, Solidity developers can ensure the robustness and reliability of their smart contracts.

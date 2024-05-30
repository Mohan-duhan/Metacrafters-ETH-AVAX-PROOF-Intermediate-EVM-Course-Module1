# 🚀 Solidity Contract Readme

📄 **Assessment.sol** - A Simple Solidity Contract for Managing Balance and Ownership

## Use of `require()`, `assert()`, and `revert()`

For this project, the smart contract implements the `require()`, `assert()`, and `revert()` statements for error handling and validation.

✅ require()

The `require()` statement is used to validate conditions before executing a function. If the condition fails, the execution stops and the transaction is reverted. It is typically used to check inputs, permissions, and other critical conditions.

Example:
```solidity
require(msg.sender == author, "You are not the author");

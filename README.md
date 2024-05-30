# 🚀 Solidity Contract Readme

📄 **Assessment.sol** - A Simple Solidity Contract for Managing Balance and Ownership

## Use of `require()`, `assert()`, and `revert()`

For this project, the smart contract implements the `require()`, `assert()`, and `revert()` statements for error handling and validation.

✅ require()

The `require()` statement is used to validate conditions before executing a function. If the condition fails, the execution stops and the transaction is reverted. It is typically used to check inputs, permissions, and other critical conditions.
Example:
```solidity
require(msg.sender == author, "You are not the author");

🔍 assert()

The assert() statement is used to check for conditions that should never be false. If the condition fails, the execution stops and the transaction is reverted. It is typically used to check for internal errors and invariants.
Example:
```solidity
assert(currBalance < previousBalance);

⚠️ revert()

The revert() statement is used to flag an error and revert the current call. It can include a message providing details about the error, which will be passed back to the caller. It is typically used to handle exceptional conditions that require halting execution and reverting state changes.
Example:
```solidity
if (currBalance < someValue) {
    revert("You do not have enough money");
}

🛠 Using the Contract in Remix IDE
To use this contract in the Remix IDE, follow these steps:

Open the Remix IDE (https://remix.ethereum.org/).
Create a new Solidity file and name it "Assessment.sol".
Copy and paste the contract code into the "Assessment.sol" file.
Select the appropriate Solidity compiler version (0.8.10 or higher) in the Remix IDE.
Compile the contract by clicking the "Compile" button.
Once compiled successfully, you can interact with the contract using the Remix IDE's built-in console or by deploying it to a test network.
Note: Before interacting with the contract, make sure you have a compatible Ethereum wallet connected to the Remix IDE (e.g., MetaMask).

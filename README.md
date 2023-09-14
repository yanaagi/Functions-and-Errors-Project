# FunctionalityContract

FunctionalityContract is a Solidity smart contract that demonstrates the usage of `require()`, `assert()`, and `revert()` statements for conditional checks and error handling.


## Overview

This smart contract includes the following functionalities:

1. Setting a contract value, with a check to ensure that only the contract owner can set the value.
2. Performing an assertion to check if two numbers are not equal.
3. Demonstrating the use of `revert()` to halt execution with a custom error message if a condition is not met.

## Functions

### `constructor()`

- The constructor sets the initial contract owner to the address that deploys the contract.

### `setValue()`

- Allows the contract owner to set the contract's value.
- Uses `require()` to ensure that only the owner can set the value.
- If the caller is not the owner, the function reverts with an error message.

### `asserts()`

- Performs an assertion using `assert()` to check if `a` is not equal to `b`.
- If the assertion fails, the contract will throw an exception.

### `reverts()`

- Demonstrates the use of `revert()` to check if `_valueToCheck` is less than 10.
- If the condition is true (i.e., `_valueToCheck` is less than 10), the function reverts with a custom error message.

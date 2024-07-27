# Initial Goals 

>[!IMPORTANT] go go cadget forge

1. Create minimal Account Abstraction on Ethereum
2. Create minimal Account Abstraction on zkSync
3. use them to deploy and send a userOp/transaction to the Ethereum network
   1. **NOTE:** will only send a transaction to the zkSync network
  
# MinimalAccount Contract for Ethereum

## Purpose

The `MinimalAccount` contract provides a simplified implementation of account abstraction for Ethereum, enabling flexible transaction validation and execution.

## Functionality

- **Transaction Validation**: Ensures that transactions can be validated by custom logic, not just a private key.
- **Execute Function**: Allows execution of calls to external contracts from the EntryPoint or the contract owner.
- **Signature Validation**: Validates signatures to confirm they match the contract owner.
- **Prefunding**: Handles prefunding for missing account funds when necessary.
- **Access Control**: Uses modifiers to restrict function calls to the EntryPoint or the contract owner.
- **EntryPoint Reference**: Stores an immutable reference to the EntryPoint contract for transaction processing.


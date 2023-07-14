---
lastUpdated: June 10, 2023
---

# Expression Rules

## Comparison operators

- ```==``` equal
- ```!=``` not equal
- ```<``` less than
- ```>``` greater than
- ```<=``` less than or equal to
- ```>=``` greater than or equal to

## Logical operators

- ```and```
- ```or```

## Array operators

- ```contain```
- ```not contain```

## General principles

An expression consists of conditions. For example, the expression ```(transaction_blockNumber == 1 or block_number == 2)``` consists of two conditions: ```(transaction_blockNumber == 1)``` and ```(block_number == 2)``` The expression can consist of one or more conditions. There have to be logical operators between the conditions.

The logical operator ```and``` means that both conditions within the expression must be true. For example, the expression ```(transaction_gas == 123 and block_number == 321)``` will be considered true, when the block number 321 will include the transaction with gas equal to 123.

The logical operator ```or```, means that at least one of the conditions must be true. For example, the expression ```(transaction_gas == 123 or block_number == 321)``` will be considered true, when the block number 321 appears on the network, or when gas is equal to 123 in any transaction.

## Principles of composing an expression

1. Substitute a prefix equivalent to the name of the Entity. For example, if you want to track the block number 42, the expression should be ```(block_number == 42)```, for transaction and receipt ```(transaction_blockNumber == 42)``` and ```(receipt_blockNumber == 42)``` respectively.
2. Such variables as int or uint must be without quotes in the expression as specified in the examples above. Such variables as hex20 и hex32 must be in double quotes, for example, ```(transaction_transactionHash == "0x91e44d7d3d8ebb0b5a9e4b0a276c0124281750182dfac5abead8efc752e6246a")```
3. Enclose the expression in round brackets.

---
title: geth:eth_call \[POST\]
description: Executes a new message call immediately, without creating a transactionon the block chain. The eth_call method can be used to query internalcontract state, to execute validations coded into a contract or even totest what the effect of a transaction would be without running it live.
---

### Parameters


`transaction` - json object

The transaction call object is mandatory.

`block` - quantity \| tag

Block number or the string latest or pending

The block number is mandatory and defines the context (state) against
which the specified transaction should be executed. It is not possible
to execute calls against reorged blocks; or blocks older than 128
(unless the node is an archive node).

`state` - json object

The state override set is an optional address-to-state mapping, where
each entry specifies some state to be ephemerally overridden prior to
executing the call. Each address maps to an object containing: -
balance - quantity - Optional, Fake balance to set for the account
before executing the call. - nonce - quantity - Optional, Fake nonce to
set for the account before executing the call. - code - binary -
Optional, Fake EVM bytecode to inject into the account before executing
the call. - state - object - Optional, Fake key-value mapping to
override all slots in the account storage before executing the call. -
stateDiff - object - Optional, Fake key-value mapping to override
individual slots in the account storage before executing the call.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_call",
"params": [[{"to": "0xebe8efa441b9302a0d7eaecc277c09d20d684540", "data": "0x0be5b6ba"}], "latest", [{"0xebe8efa441b9302a0d7eaecc277c09d20d684540": {"code": "0x6080604052348015600f57600080fd5b506004361060285760003560e01c80630be5b6ba14602d575b600080fd5b60336045565b60408051918252519081900360200190f35b6007549056fea265627a7a723058206f26bd0433456354d8d1228d8fe524678a8aeeb0594851395bdbd35efc2a65f164736f6c634300050a0032"}}]],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0000000000000000000000000000000000000000000000000000000000000002"
}
```


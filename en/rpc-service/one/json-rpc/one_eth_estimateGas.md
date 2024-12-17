---
title: one:eth_estimateGas \[POST\]
description: Returns an estimate of the gas required for a transaction to complete.The estimation process does not use gas and the transaction is not addedto the blockchain. The resulting estimate can be greater than the amountof gas the transaction ends up using, for reasons including EVMmechanics and node performance.The eth_estimateGas call does not send a transaction. You must calleth_sendRawTransaction to execute the transaction.If revert reason is enabled with --revert-reason-enabled, theeth_estimateGas error response will include the revert reason.
---

### Parameters


`object` - object

Transaction call object.

### Request

``` java
curl --location --request POST 'https://one.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_estimateGas",
"params": [{"from": "0xFE3B557E8Fb62b89F4916B721be55cEb828dBd73", "to": "0x44Aa93095D6749A706051658B970b941c72c1D53", "value": "0x1"}],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x5208"
}
```


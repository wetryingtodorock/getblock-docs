---
title: avax:avax.getAtomicTxStatus  {disallowed} - Avalanche
description: Example code for the avax:avax.getAtomicTxStatus  {disallowed} ws method. Сomplete guide on how to use avax:avax.getAtomicTxStatus  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`txID` - string

id of the transaction

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "avax.getAtomicTxStatus",
"params": [null],
"id": "getblock.io"}
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```


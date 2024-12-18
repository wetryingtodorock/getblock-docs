---
title: avax.getAtomicTx  {disallowed} - Avalanche
description: Example code for the avax.getAtomicTx  {disallowed} ws method. Сomplete guide on how to use avax.getAtomicTx  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`txID` - string

txID is the transacion ID. It should be in cb58 format.

`encoding` - string

Optional encoding parameter to specify the format for the returned
transaction. Can be either cb58 or hex. Defaults to cb58.

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "avax.getAtomicTx",
"params": [null, null],
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


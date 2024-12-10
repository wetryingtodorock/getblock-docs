---
title: avax:eth_compileSolidity  {disallowed} - Avalanche
description: Example code for the avax:eth_compileSolidity  {disallowed} ws method. Сomplete guide on how to use avax:eth_compileSolidity  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`code` - string

The source code.

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_compileSolidity",
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


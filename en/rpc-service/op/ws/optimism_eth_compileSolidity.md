---
title: optimism:eth_compileSolidity  {disallowed} - Optimism
description: Example code for the optimism:eth_compileSolidity  {disallowed} ws method. Сomplete guide on how to use optimism:eth_compileSolidity  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`code` - string

The source code.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
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


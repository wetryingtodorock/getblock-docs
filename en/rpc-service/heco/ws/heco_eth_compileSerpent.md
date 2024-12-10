---
title: heco:eth_compileSerpent  {disallowed} - Huobi ECO Chain
description: Example code for the heco:eth_compileSerpent  {disallowed} ws method. Сomplete guide on how to use heco:eth_compileSerpent  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`code` - string

The source code.

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_compileSerpent",
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


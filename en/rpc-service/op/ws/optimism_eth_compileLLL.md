---
title: optimism:eth_compileLLL  {disallowed} - Optimism
description: Example code for the optimism:eth_compileLLL  {disallowed} ws method. Сomplete guide on how to use optimism:eth_compileLLL  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`code` - string

The source code.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_compileLLL",
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


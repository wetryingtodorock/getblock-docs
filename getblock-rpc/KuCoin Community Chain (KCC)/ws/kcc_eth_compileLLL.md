---
title: eth_compileLLL  {disallowed} - KuCoin Community Chain
description: Example code for the eth_compileLLL  {disallowed} ws method. Сomplete guide on how to use eth_compileLLL  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`code` - string

The source code.

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
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


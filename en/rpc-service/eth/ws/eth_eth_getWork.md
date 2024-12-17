---
title: eth:eth_getWork - Ethereum
description: Example code for the eth:eth_getWork ws method. Сomplete guide on how to use eth:eth_getWork ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getWork",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "no mining work available yet"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```


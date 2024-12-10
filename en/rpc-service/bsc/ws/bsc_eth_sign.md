---
title: bsc:eth_sign - Binance Smart Chain
description: Example code for the bsc:eth_sign ws method. Сomplete guide on how to use bsc:eth_sign ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - hex string

20 Bytes - address

`DATA` - hex string

N Bytes - message to sign

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_sign",
"params": ["0xcee8ae756461e2653b88aefdbd70c1144de52b23", "0xbcda"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "unknown account"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```


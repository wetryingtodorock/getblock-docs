---
title: arbitrum:eth_sign - Arbitrum
description: Example code for the arbitrum:eth_sign ws method. Сomplete guide on how to use arbitrum:eth_sign ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address.

`DATA` - string

message to sign.

### Request

``` java
wscat -c wss://arbitrum.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_sign",
"params": ["0x9b956e3d318625be2686ae7268d81777c462d41f", "0xdeadbeaf"],
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


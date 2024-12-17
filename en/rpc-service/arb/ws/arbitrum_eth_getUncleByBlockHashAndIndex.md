---
title: arbitrum:eth_getUncleByBlockHashAndIndex - Arbitrum
description: Example code for the arbitrum:eth_getUncleByBlockHashAndIndex ws method. Сomplete guide on how to use arbitrum:eth_getUncleByBlockHashAndIndex ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

Hash of a block.

`QUANTITY` - string

the uncle’s index position.

### Request

``` java
wscat -c wss://arbitrum.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockHashAndIndex",
"params": ["0xf5524f0cf99ac6bc5905e95294ebed9007e2d978155f3457118eb7a26d97503a", "0x0"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": null
}
```


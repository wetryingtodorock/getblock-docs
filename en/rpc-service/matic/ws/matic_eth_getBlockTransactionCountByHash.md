---
title: matic:eth_getBlockTransactionCountByHash - Polygon
description: Example code for the matic:eth_getBlockTransactionCountByHash ws method. Сomplete guide on how to use matic:eth_getBlockTransactionCountByHash ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

hash of the block.

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByHash",
"params": ["0x81e807e7a6031d9f103eeee2a2edc5994c3432ee1e3227c66ff78eef30ea1dec"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x76"
}
```


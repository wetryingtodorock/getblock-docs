---
title: heco:eth_getUncleCountByBlockHash - Huobi ECO Chain
description: Example code for the heco:eth_getUncleCountByBlockHash ws method. Сomplete guide on how to use heco:eth_getUncleCountByBlockHash ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

hash of the block.

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockHash",
"params": ["0x779f94a2fad68383ed932e9f8fd04234a92b85f9d849bec2188c675dcdb0f16d"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0"
}
```


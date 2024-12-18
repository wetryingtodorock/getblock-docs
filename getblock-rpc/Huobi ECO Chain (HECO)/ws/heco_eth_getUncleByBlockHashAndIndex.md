---
title: eth_getUncleByBlockHashAndIndex - Huobi ECO Chain
description: Example code for the eth_getUncleByBlockHashAndIndex ws method. Сomplete guide on how to use eth_getUncleByBlockHashAndIndex ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

Hash of a block.

`QUANTITY` - string

the uncle’s index position.

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockHashAndIndex",
"params": ["0x779f94a2fad68383ed932e9f8fd04234a92b85f9d849bec2188c675dcdb0f16d", "0x0"],
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


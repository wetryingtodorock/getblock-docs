---
title: matic:eth_getUncleByBlockHashAndIndex \[WebSocket\]
description: Returns information about a uncle of a block by hash and uncle indexposition.
---

### Parameters


`DATA` - string

Hash of a block.

`QUANTITY` - string

the uncle’s index position.

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockHashAndIndex",
"params": ["0x81e807e7a6031d9f103eeee2a2edc5994c3432ee1e3227c66ff78eef30ea1dec", "0x0"],
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


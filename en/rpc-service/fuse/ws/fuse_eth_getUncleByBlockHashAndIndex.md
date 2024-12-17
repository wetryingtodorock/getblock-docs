---
title: fuse:eth_getUncleByBlockHashAndIndex \[WebSocket\]
description: Returns information about a uncle of a block by hash and uncle indexposition.
---

### Parameters


`DATA` - string

Hash of a block.

`QUANTITY` - string

the uncle’s index position.

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockHashAndIndex",
"params": ["0x21056b00f69c1d8f9e0caf94914efe3119cb1668163a9e432c01a9f900e37249", "0x0"],
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


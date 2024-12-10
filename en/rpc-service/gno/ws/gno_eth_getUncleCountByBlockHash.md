---
title: gno:eth_getUncleCountByBlockHash - Gnosis
description: Example code for the gno:eth_getUncleCountByBlockHash ws method. Сomplete guide on how to use gno:eth_getUncleCountByBlockHash ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - None

32-byte block hash.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockHash",
"params": ["0xc11de1b67dd435ada2b83bbf0bb45cba5efab4e8dd00b100142e799ba902dddc"],
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


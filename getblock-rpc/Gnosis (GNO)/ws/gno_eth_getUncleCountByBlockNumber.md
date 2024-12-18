---
title: eth_getUncleCountByBlockNumber - Gnosis
description: Example code for the eth_getUncleCountByBlockNumber ws method. Сomplete guide on how to use eth_getUncleCountByBlockNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - None

Integer representing either the index of the block within the
blockchain, or one of the string tags latest, earliest, or pending, as
described in Block Parameter.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockNumber",
"params": ["0x1BC4"],
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


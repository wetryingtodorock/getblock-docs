---
title: rsk:eth_getUncleCountByBlockNumber \[WebSocket\]
description: Returns the number of uncles in a block from a block matching the givenblock number.
---

### Parameters


`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockNumber",
"params": ["latest"],
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


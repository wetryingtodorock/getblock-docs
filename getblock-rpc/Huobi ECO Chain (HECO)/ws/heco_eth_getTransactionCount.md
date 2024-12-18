---
title: eth_getTransactionCount - Huobi ECO Chain
description: Example code for the eth_getTransactionCount ws method. Сomplete guide on how to use eth_getTransactionCount ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address.

`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getTransactionCount",
"params": ["0xb0660a58f97733636b7555162b62e0e83786f79c", "latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x4f"
}
```


---
title: heco:eth_getBalance - Huobi ECO Chain
description: Example code for the heco:eth_getBalance ws method. Сomplete guide on how to use heco:eth_getBalance ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address to check for balance.

`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0xb0660a58f97733636b7555162b62e0e83786f79c", "latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xe3f1535988400"
}
```


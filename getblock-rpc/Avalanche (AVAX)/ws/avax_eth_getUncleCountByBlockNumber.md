---
title: eth_getUncleCountByBlockNumber - Avalanche
description: Example code for the eth_getUncleCountByBlockNumber ws method. Сomplete guide on how to use eth_getUncleCountByBlockNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
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


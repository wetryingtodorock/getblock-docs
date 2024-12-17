---
title: avax:eth_getBalance - Avalanche
description: Example code for the avax:eth_getBalance ws method. Сomplete guide on how to use avax:eth_getBalance ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address to check for balance.

`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0x0f8d94cea1eba9c582bbe800545ca91dfc39da18", "latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x2fe10fc87c0ae5"
}
```


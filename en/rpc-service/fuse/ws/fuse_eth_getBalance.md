---
title: fuse:eth_getBalance - Fuse Network
description: Example code for the fuse:eth_getBalance ws method. Сomplete guide on how to use fuse:eth_getBalance ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address to check for balance.

`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0x9b956e3d318625be2686ae7268d81777c462d41f", "latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x45c2e7deff1d6a01"
}
```


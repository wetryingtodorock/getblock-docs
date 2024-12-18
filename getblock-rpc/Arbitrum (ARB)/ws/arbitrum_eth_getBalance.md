---
title: eth_getBalance - Arbitrum
description: Example code for the eth_getBalance ws method. Сomplete guide on how to use eth_getBalance ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address to check for balance.

`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://arbitrum.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0xb8b2522480f850eb198ada5c3f31ac528538d2f5", "latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x153b785d20e80ac"
}
```


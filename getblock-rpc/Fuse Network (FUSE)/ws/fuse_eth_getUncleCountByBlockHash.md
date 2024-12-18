---
title: eth_getUncleCountByBlockHash - Fuse Network
description: Example code for the eth_getUncleCountByBlockHash ws method. Сomplete guide on how to use eth_getUncleCountByBlockHash ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

hash of the block.

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockHash",
"params": ["0x360c79467da57c8db35624484cabbca4d9fc7a7813f194f5391639d2e2c39023"],
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


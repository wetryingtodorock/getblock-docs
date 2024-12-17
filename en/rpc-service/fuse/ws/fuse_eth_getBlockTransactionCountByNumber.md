---
title: fuse:eth_getBlockTransactionCountByNumber - Fuse Network
description: Example code for the fuse:eth_getBlockTransactionCountByNumber ws method. Сomplete guide on how to use fuse:eth_getBlockTransactionCountByNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByNumber",
"params": ["latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x1"
}
```


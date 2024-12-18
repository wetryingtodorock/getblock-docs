---
title: eth_getBlockTransactionCountByNumber - Avalanche
description: Example code for the eth_getBlockTransactionCountByNumber ws method. Сomplete guide on how to use eth_getBlockTransactionCountByNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "0x11"
}
```


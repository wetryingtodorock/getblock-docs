---
title: eth_getTransactionCount - Avalanche
description: Example code for the eth_getTransactionCount ws method. Сomplete guide on how to use eth_getTransactionCount ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address.

`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getTransactionCount",
"params": ["0x0f8d94cea1eba9c582bbe800545ca91dfc39da18", "earliest"],
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


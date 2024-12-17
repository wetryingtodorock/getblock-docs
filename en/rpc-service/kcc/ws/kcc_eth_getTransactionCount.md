---
title: kcc:eth_getTransactionCount - KuCoin Community Chain
description: Example code for the kcc:eth_getTransactionCount ws method. Сomplete guide on how to use kcc:eth_getTransactionCount ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address.

`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getTransactionCount",
"params": ["0xbec4e80531dad6a9989828d174cc2878b1e3123d", "earliest"],
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


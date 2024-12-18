---
title: eth_getBlockTransactionCountByNumber - KuCoin Community Chain
description: Example code for the eth_getBlockTransactionCountByNumber ws method. Сomplete guide on how to use eth_getBlockTransactionCountByNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByNumber",
"params": ["0xc6f437"],
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


---
title: kcc:eth_getUncleByBlockNumberAndIndex - KuCoin Community Chain
description: Example code for the kcc:eth_getUncleByBlockNumberAndIndex ws method. Сomplete guide on how to use kcc:eth_getUncleByBlockNumberAndIndex ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

`QUANTITY` - string

the uncle’s index position.

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockNumberAndIndex",
"params": ["latest", "0x0"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": null
}
```


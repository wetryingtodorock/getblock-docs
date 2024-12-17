---
title: optimism:eth_getBalance \[WebSocket\]
description: Returns the balance of the account of given address.
---

### Parameters


`DATA` - string

address to check for balance.

`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0xbec4e80531dad6a9989828d174cc2878b1e3123d", "latest"],
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


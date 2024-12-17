---
title: optimism:eth_getTransactionCount \[WebSocket\]
description: Returns the number of transactions sent from an address.
---

### Parameters


`DATA` - string

address.

`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
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


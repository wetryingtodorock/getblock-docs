---
title: optimism:eth_getStorageAt - Optimism
description: Example code for the optimism:eth_getStorageAt ws method. Сomplete guide on how to use optimism:eth_getStorageAt ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address to check for balance.

`QUANTITY` - integer

Position in the storage.

`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getStorageAt",
"params": ["0xbec4e80531dad6a9989828d174cc2878b1e3123d", "0x0", "earliest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0000000000000000000000000000000000000000000000000000000000000000"
}
```


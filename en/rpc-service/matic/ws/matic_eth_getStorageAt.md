---
title: matic:eth_getStorageAt - Polygon
description: Example code for the matic:eth_getStorageAt ws method. Сomplete guide on how to use matic:eth_getStorageAt ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address to check for balance.

`QUANTITY` - integer

Position in the storage.

`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getStorageAt",
"params": ["0xe7e2cb8c81c10ff191a73fe266788c9ce62ec754", "0x01", "latest"],
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


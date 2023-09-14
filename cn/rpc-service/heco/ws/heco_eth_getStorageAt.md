---
title: heco:eth_getStorageAt \[WebSocket\]
description: Returns the value from a storage position at a given address.
---

### Parameters


`DATA` - string

address to check for balance.

`QUANTITY` - string

Position in the storage.

`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getStorageAt",
"params": ["0xb0660a58f97733636b7555162b62e0e83786f79c", "0x0", "latest"],
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


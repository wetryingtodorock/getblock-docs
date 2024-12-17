---
title: fuse:eth_getStorageAt \[POST\]
description: Returns the value from a storage position at a given address.
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
curl --location --request POST 'https://fuse.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getStorageAt",
"params": ["0x9b956e3d318625be2686ae7268d81777c462d41f", "0x0", "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0000000000000000000000000000000000000000000000000000000000000000"
}
```


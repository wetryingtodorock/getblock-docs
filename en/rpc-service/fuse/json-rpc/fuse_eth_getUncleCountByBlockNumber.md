---
title: fuse:eth_getUncleCountByBlockNumber - Fuse Network
description: Example code for the fuse:eth_getUncleCountByBlockNumber json-rpc method. Сomplete guide on how to use fuse:eth_getUncleCountByBlockNumber json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

### Request

``` java
curl --location --request POST 'https://fuse.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockNumber",
"params": ["latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0"
}
```


---
title: eth_getUncleByBlockNumberAndIndex - Polygon
description: Example code for the eth_getUncleByBlockNumberAndIndex json-rpc method. Сomplete guide on how to use eth_getUncleByBlockNumberAndIndex json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

`QUANTITY` - string

the uncle’s index position.

### Request

``` java
curl --location --request POST 'https://matic.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockNumberAndIndex",
"params": ["latest", "0x0"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": null
}
```


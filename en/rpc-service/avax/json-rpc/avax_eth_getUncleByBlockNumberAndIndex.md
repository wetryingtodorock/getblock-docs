---
title: avax:eth_getUncleByBlockNumberAndIndex - Avalanche
description: Example code for the avax:eth_getUncleByBlockNumberAndIndex json-rpc method. Сomplete guide on how to use avax:eth_getUncleByBlockNumberAndIndex json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

`QUANTITY` - string

the uncle’s index position.

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
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


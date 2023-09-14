---
title: ftm:eth_getUncleByBlockNumberAndIndex \[POST\]
description: Returns uncle specified by block number and index.
---

### Parameters


`quantity|tag` - hex string

Index of the block, or one of the string tags latest, earliest, or
pending, as described in Block Parameter.

`quantity` - hex string

Index of the uncle.

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockNumberAndIndex",
"params": ["0x89D2", "0x0"],
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


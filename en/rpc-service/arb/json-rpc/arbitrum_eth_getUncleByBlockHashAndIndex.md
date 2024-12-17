---
title: arbitrum:eth_getUncleByBlockHashAndIndex \[POST\]
description: Returns information about a uncle of a block by hash and uncle indexposition.
---

### Parameters


`DATA` - string

Hash of a block.

`QUANTITY` - string

the uncle’s index position.

### Request

``` java
curl --location --request POST 'https://arbitrum.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockHashAndIndex",
"params": ["0xf5524f0cf99ac6bc5905e95294ebed9007e2d978155f3457118eb7a26d97503a", "0x0"],
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


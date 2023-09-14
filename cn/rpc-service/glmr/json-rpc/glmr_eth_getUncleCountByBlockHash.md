---
title: glmr:eth_getUncleCountByBlockHash \[POST\]
description: Returns the number of uncles in a block from a block matching the givenblock hash.
---

### Parameters


`DATA` - string

hash of the block.

### Request

``` java
curl --location --request POST 'https://glmr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockHash",
"params": ["0xe21d18d5b511b13c66b4d162111b5d41646782378ee35eb208b62be36942a859"],
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


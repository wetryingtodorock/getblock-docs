---
title: etc:eth_getUncleCountByBlockHash \[POST\]
description: Returns the number of uncles in a block from a block matching the givenblock hash.
---

### Parameters


`DATA` - string

32-byte block hash.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockHash",
"params": ["0xbb50cb8d2d5698c1b10f1a845360ecf521ff18b08f71664a4639b6bdbb08fb38"],
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


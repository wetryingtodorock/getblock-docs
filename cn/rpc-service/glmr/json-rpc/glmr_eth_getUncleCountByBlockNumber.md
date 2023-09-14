---
title: glmr:eth_getUncleCountByBlockNumber \[POST\]
description: Returns the number of uncles in a block from a block matching the givenblock number.
---

### Parameters


`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
curl --location --request POST 'https://glmr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockNumber",
"params": ["0xc6f437"],
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


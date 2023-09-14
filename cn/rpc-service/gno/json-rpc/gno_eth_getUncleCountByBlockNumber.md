---
title: gno:eth_getUncleCountByBlockNumber \[POST\]
description: Returns the number of uncles in a block matching the specified blocknumber.
---

### Parameters


`QUANTITY|TAG` - None

Integer representing either the index of the block within the
blockchain, or one of the string tags latest, earliest, or pending, as
described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://gno.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockNumber",
"params": ["0x1BC4"],
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


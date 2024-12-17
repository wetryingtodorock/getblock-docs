---
title: near:gas_price \[POST\]
description: Returns gas price for a specific block_height or block_hash.Using \[null\] will return the most recent blocks gas price.
---

### Parameters


`block` - int or string

Optional

block height or block hash.

### Request

``` java
curl --location --request POST 'https://near.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "gas_price",
"params": [61067007],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "gas_price": "100000000"
    }
}
```


---
title: near:gas_price - NEAR Protocol
description: Example code for the near:gas_price json-rpc method. Сomplete guide on how to use near:gas_price json-rpc in GetBlock.io Web3 documentation.
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


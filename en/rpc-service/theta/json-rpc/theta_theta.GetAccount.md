---
title: theta:theta.GetAccount \[POST\]
description: This API returns the details of the account being queried in jsonformat.
---

### Parameters


`address` - string

the address of the account.

### Request

``` java
curl --location --request POST 'https://theta.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "theta.GetAccount",
"params": {"address": "0x4b80a68a8469d33449eb101082e5500b932a23ce"},
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "code": "0xc5d2460186f7233c927e7db2dcc703c0e500b653ca82273b7bfad8045d85a470",
        "coins": {
            "tfuelwei": "0",
            "thetawei": "0"
        },
        "last_updated_block_height": "0",
        "reserved_funds": [],
        "root": "0x0000000000000000000000000000000000000000000000000000000000000000",
        "sequence": "0"
    }
}
```


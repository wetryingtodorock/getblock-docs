---
title: ont:getmempooltxstate \[POST\]
description: Fetch state of transaction in the node memory pool using giventransaction hash.
---

### Parameters


`hash` - string

transaction hash

### Request

``` java
curl --location --request POST 'https://ont.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getmempooltxstate",
"params": ["db81c4e00f050c4f8e2f9c7e8201fddebd18458b3c48c73c18aa0532c7b5c43c"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "desc": "SUCCESS",
    "error": 0,
    "jsonrpc": "2.0",
    "id": 1,
    "result": {
        "State": [
            {
                "Type": 1,
                "Height": 342,
                "ErrCode": 0
            },
            {
                "Type": 0,
                "Height": 0,
                "ErrCode": 0
            }
        ]
    }
}
```


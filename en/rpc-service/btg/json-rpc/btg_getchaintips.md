---
title: btg:getchaintips \[POST\]
description: Return information about all known tips in the block tree, including themain chain as well as orphaned branches.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getchaintips",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": [
        {
            "branchlen": 0,
            "hash": "000000007cc1fc836d0992202730ca71f77a8cf2a35974ca300dadbf8bc1e090",
            "height": 702634,
            "status": "active"
        }
    ]
}
```


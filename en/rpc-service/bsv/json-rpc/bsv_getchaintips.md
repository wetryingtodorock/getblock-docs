---
title: bsv:getchaintips \[POST\]
description: Return information about all known tips in the block tree, including themain chain as well as orphaned branches.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
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
            "hash": "0000000000000000023a561e1ea370153aac5d1504726d1a039032831c05fcfc",
            "height": 684634,
            "status": "active"
        },
        {
            "branchlen": 1,
            "hash": "000000000000000001d3a318372df5d1eec54462a0d7471ae1cdf49838f793dd",
            "height": 683516,
            "status": "valid-headers"
        }
    ]
}
```


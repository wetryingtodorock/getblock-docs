---
title: btc:getindexinfo \[POST\]
description: Returns the status of one or all available indices currently running inthe node.
---

### Parameters


`index_name` - string, optional

Filter results for an index with a specific name.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getindexinfo",
"params": ["default"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": {
        "txindex": {
            "synced": true,
            "best_block_height": 680586
        },
        "basic block filter index": {
            "synced": true,
            "best_block_height": 680586
        }
    },
    "error": null,
    "id": "getblock.io"
}
```


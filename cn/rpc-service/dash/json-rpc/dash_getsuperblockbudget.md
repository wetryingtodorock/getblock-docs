---
title: dash:getsuperblockbudget \[POST\]
description: returns the absolute maximum sum of superblock payments allowed.
---

### Parameters


`index` - number (int)

The superblock index.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getsuperblockbudget",
"params": [1528672],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": 4945.4258956
}
```


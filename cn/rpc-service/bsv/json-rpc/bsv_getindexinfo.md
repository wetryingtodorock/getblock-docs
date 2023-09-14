---
title: bsv:getindexinfo \[POST\]
description: Returns the status of one or all available indices currently running inthe node.
---

### Parameters


`index_name` - string, optional

Filter results for an index with a specific name.

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
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
    "error": null,
    "id": "getblock.io",
    "result": {}
}
```


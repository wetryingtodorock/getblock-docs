---
title: zec:estimatefee \[POST\]
description: Estimates the approximate fee per kilobyte needed for a transaction tobegin confirmation within nblocks blocks.
---

### Parameters


`nblocks` - numeric

None

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "estimatefee",
"params": [5],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": 0.0001005
}
```


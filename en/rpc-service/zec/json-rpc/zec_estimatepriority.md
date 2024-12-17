---
title: zec:estimatepriority \[POST\]
description: Estimates the approximate priority a zero-fee transaction needs to beginconfirmation within nblocks blocks.
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
"method": "estimatepriority",
"params": [5],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": -1
}
```


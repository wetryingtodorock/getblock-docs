---
title: bsv:getblockhash - Bitcoin SV
description: Example code for the bsv:getblockhash json-rpc method. Сomplete guide on how to use bsv:getblockhash json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`height` - numeric, required

The height index

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getblockhash",
"params": [1000],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "00000000c937983704a73af28acdec37b049d214adbda81d7e2a3dd146f6ed09"
}
```


---
title: bsv:removeprunedfunds  {disallowed} - Bitcoin SV
description: Example code for the bsv:removeprunedfunds  {disallowed} json-rpc method. Сomplete guide on how to use bsv:removeprunedfunds  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`txid` - string, required

The hex-encoded id of the transaction you are deleting

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "removeprunedfunds",
"params": [null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```


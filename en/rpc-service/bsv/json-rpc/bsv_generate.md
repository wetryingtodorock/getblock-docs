---
title: bsv:generate  {disallowed} - Bitcoin SV
description: Example code for the bsv:generate  {disallowed} json-rpc method. Сomplete guide on how to use bsv:generate  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`nblocks` - numeric, required

How many blocks are generated immediately.

`maxtries` - numeric, optional, default=1000000

How many iterations to try.

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "generatetodescriptor",
"params": [null, null, null],
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


---
title: bsv:getnodeaddresses  {disallowed} - Bitcoin SV
description: Example code for the bsv:getnodeaddresses  {disallowed} json-rpc method. Сomplete guide on how to use bsv:getnodeaddresses  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`count` - numeric, optional, default=1

How many addresses to return. Limited to the smaller of 2500 or 23% of
all known addresses.

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getnodeaddresses",
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


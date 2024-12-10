---
title: bsv:submitblocklight  {disallowed} - Bitcoin SV
description: Example code for the bsv:submitblocklight  {disallowed} json-rpc method. Сomplete guide on how to use bsv:submitblocklight  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`hexdata` - string, required

The hex-encoded block data to submit. The block must have exactly 1
transaction (coinbase). Additional transactions (if any) are appended
from the light template.

`job_id` - string, required

Identifier of the light template from which to retrieve the non-coinbase
transactions. This job_id must be obtained from a previous call to
getblocktemplatelight.

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "submitblocklight",
"params": [null, null],
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


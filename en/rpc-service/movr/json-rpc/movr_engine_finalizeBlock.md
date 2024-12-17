---
title: movr:engine_finalizeBlock \[POST\] {disallowed}
description: Instructs the manual-seal authorship task to finalize a block.
---

### Parameters


`hash` - BlockHash

None

`justification` - Justification

None

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "engine_finalizeBlock",
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


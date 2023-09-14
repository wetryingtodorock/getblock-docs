---
title: movr:engine_createBlock \[POST\] {disallowed}
description: Instructs the manual-seal authorship task to create a new block.
---

### Parameters


`createEmpty` - bool

None

`finalize` - bool

None

`parentHash` - BlockHash

None

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "engine_createBlock",
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


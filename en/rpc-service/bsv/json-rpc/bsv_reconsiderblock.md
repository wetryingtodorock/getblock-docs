---
title: bsv:reconsiderblock \[POST\] {disallowed}
description: Removes invalidity status of a block and its descendants, reconsiderthem for activation.This can be used to undo the effects of invalidateblock.
---

### Parameters


`blockhash` - string, required

the hash of the block to reconsider

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "reconsiderblock",
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


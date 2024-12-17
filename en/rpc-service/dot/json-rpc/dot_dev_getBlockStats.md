---
title: dot:dev_getBlockStats \[POST\] {disallowed}
description: Reexecute the specified block_hash and gather statistics while doing soThis method is only active with appropriate flags
---

### Parameters


`at` - Hash

block hash

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "dev_getBlockStats",
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


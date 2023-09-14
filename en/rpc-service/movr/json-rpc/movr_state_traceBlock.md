---
title: movr:state_traceBlock \[POST\] {disallowed}
description: Provides a way to trace the re-execution of a single block
---

### Parameters


`block` - Hash

block hash

`targets` - Option Text

target

`StorageKey` - Option Text

storage key

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "state_traceBlock",
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


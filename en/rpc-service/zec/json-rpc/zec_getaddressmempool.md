---
title: zec:getaddressmempool \[POST\] {disallowed}
description: Returns all mempool deltas for an address.WARNING getaddressmempool is disabled.
---

### Parameters


`addresses` - list of string

List of the base58check encoded addresses

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getaddressmempool",
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


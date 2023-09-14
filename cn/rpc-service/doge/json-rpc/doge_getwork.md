---
title: doge:getwork \[POST\] {disallowed}
description: Get work for remote mining, or submit result. If data is specified, theserver tries to solve the block using the provided data and returns Trueif it was successful. If not, the function returns formatted hash data(WorkItem) to work on.
---

### Parameters


`data` - string

Optional.

Result from remote mining.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getwork",
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


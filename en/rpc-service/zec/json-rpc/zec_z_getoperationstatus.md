---
title: zec:z_getoperationstatus \[POST\] {disallowed}
description: Get operation status and any associated result or error data. Theoperation will remain in memory.
---

### Parameters


`operationid` - array

Optional

A list of operation ids we are interested in. If not provided, examine
all operations known to the node.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_getoperationstatus",
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


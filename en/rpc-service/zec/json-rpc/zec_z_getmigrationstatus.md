---
title: zec:z_getmigrationstatus \[POST\] {disallowed}
description: Returns information about the status of the Sprout to Sapling migration.Note A transaction is defined as finalized if it has at least tenconfirmations.Also, it is possible that manually created transactions involving thiswallet will be included in the result.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_getmigrationstatus",
"params": [],
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


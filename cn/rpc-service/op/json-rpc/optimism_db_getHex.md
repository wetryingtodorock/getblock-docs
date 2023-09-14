---
title: optimism:db_getHex \[POST\] {disallowed}
description: Returns binary data from the local database.Note this function is deprecated and will be removed in the future.
---

### Parameters


`database` - string

Database name

`key` - string

key name

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "db_getHex",
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


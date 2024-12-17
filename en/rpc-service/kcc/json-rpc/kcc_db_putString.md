---
title: kcc:db_putString \[POST\] {disallowed}
description: Stores a string in the local database.Note this function is deprecated and will be removed in the future.
---

### Parameters


`database` - string

database name

`key` - string

key name

`string` - string

string to store.

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "db_putString",
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


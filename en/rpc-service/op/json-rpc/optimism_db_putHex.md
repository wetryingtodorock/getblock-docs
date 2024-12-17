---
title: optimism:db_putHex \[POST\] {disallowed}
description: Stores binary data in the local database.Note this function is deprecated and will be removed in the future.
---

### Parameters


`database` - string

database name

`key` - string

key name

`data` - data

data to store.

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "db_putHex",
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


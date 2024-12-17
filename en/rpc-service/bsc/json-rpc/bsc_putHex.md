---
title: bsc:putHex \[POST\] {disallowed}
description: Stores binary data in the local database.Note this function is deprecated and will be removed in the future.
---

### Parameters


`String` - None

Database name

`String` - None

Key name

`DATA` - None

The data to store

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "putHex",
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


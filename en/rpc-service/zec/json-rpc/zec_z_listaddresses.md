---
title: zec:z_listaddresses \[POST\] {disallowed}
description: Returns the list of Sprout and Sapling shielded addresses belonging tothe wallet.
---

### Parameters


`includeWatchonly` - boolean

Optional, default=false

Also include watchonly addresses.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_listaddresses",
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


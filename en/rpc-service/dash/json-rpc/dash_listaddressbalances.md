---
title: dash:listaddressbalances \[POST\] {disallowed}
description: Lists addresses of this wallet and their balances.
---

### Parameters


`Minimum Amount` - numeric (int)

Optional.

Minimum balance in DASH an address should have to be shown in the list
(default=0).

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "listaddressbalances",
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


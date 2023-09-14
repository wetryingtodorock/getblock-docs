---
title: neo:getnep17balances \[POST\] {disallowed}
description: Returns the balance of all NEP17 assets in the specified address.
---

### Parameters


`address` - string

The address that you want to query balance.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getnep17balances",
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


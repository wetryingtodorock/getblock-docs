---
title: zec:z_gettotalbalance \[POST\] {disallowed}
description: Return the total value of funds stored in the nodes wallet.CAUTION If the wallet contains any addresses for which it only hasincoming viewing keys, the returned private balance may be larger thanthe actual balance, because spends cannot be detected with incomingviewing keys.
---

### Parameters


`minconf` - numeric

Optional, default=1

Only include private and transparent transactions confirmed at least
this many times.

`includeWatchonly` - boolean

Optional, default=false

Also include balance in watchonly addresses.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_gettotalbalance",
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


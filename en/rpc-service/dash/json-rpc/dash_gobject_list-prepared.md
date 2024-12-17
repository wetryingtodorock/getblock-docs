---
title: dash:gobject_list-prepared \[POST\] {disallowed}
description: returns a list of governance objects prepared by this wallet withgobject prepare sorted by their creation time.
---

### Parameters


`method name` - string

None

`count` - number (int)

Optional

Maximum number of objects to return.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "gobject",
"params": ["list-prepared", null],
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


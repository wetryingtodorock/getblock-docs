---
title: dash:gobject_submit \[POST\] {disallowed}
description: Submits a governance object to network (objects must first be preparedvia gobject prepare).
---

### Parameters


`method name` - string

None

`parent-hash` - string (hex)

Hash of the parent object. Usually the root node which has a hash of 0

`revision` - int

Object revision number

`time` - int_64t

Create time (Unix epoch time)

`data-hex` - string (hex)

Updated in Dash Core 0.14.0 to require all new proposals to use JSON
serialization.

Object data (JSON object with governance details).

`data` - string (hex)

Fee transaction ID - required for all objects except triggers.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "gobject",
"params": ["submit", null, null, null, null, null],
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


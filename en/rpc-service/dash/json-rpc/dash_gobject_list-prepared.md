---
title: dash:gobject_list-prepared  {disallowed} - Dash
description: Example code for the dash:gobject_list-prepared  {disallowed} json-rpc method. Сomplete guide on how to use dash:gobject_list-prepared  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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


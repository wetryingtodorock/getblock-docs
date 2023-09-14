---
title: dash:gobject_count \[POST\]
description: returns the count of governance objects and votes.
---

### Parameters


`method name` - string

None

`mode` - string

Result return format:

\- json (default)

\- all - Default before Dash Core 0.12.3 (for backwards compatibility)

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "gobject",
"params": ["count", "json"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "erased": 36,
        "objects_total": 14,
        "other": 0,
        "proposals": 14,
        "triggers": 0,
        "votes": 11078
    }
}
```


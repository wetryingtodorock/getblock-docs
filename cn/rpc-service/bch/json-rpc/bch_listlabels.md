---
title: bch:listlabels \[POST\] {disallowed}
description: Returns the list of all labels, or labels that are assigned to addresseswith a specific purpose.
---

### Parameters


`purpose` - string, optional

Address purpose to list labels for (‘send’,’receive’). An empty string
is the same as not providing this argument.

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "listlabels",
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


---
title: bch:setlabel \[POST\] {disallowed}
description: Sets the label associated with the given address.
---

### Parameters


`address` - string, required

The bitcoin address to be associated with a label.

`label` - string, required

The label to assign to the address.

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "setlabel",
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


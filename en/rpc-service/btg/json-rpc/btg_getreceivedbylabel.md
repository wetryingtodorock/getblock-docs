---
title: btg:getreceivedbylabel \[POST\] {disallowed}
description: Returns the total amount received by addresses with label intransactions with at least \[minconf\] confirmations.
---

### Parameters


`label` - string, required

The selected label, may be the default label using “”.

`minconf` - numeric, optional, default=1

Only include transactions confirmed at least this many times.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getreceivedbylabel",
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


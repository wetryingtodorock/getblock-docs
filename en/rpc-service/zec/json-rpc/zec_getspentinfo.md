---
title: zec:getspentinfo \[POST\] {disallowed}
description: Returns the txid and index where an output is spent.WARNING getspentinfo is disabled.
---

### Parameters


`txid` - string

The hex string of the txid.

`index` - number

The vout (output) index.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getspentinfo",
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


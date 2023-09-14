---
title: dash:importelectrumwallet \[POST\] {disallowed}
description: Imports keys from an Electrum wallet export file (.csv or .json)
---

### Parameters


`File name` - string

The Electrum wallet export file (should be in csv or json format).

`Index` - number (int)

Optional.

Rescan the wallet for transactions starting from this block index
(default: 0)

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "importelectrumwallet",
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


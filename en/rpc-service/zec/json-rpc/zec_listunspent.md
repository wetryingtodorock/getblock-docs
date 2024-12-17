---
title: zec:listunspent \[POST\] {disallowed}
description: Returns array of unspent transaction outputs with between minconf andmaxconf (inclusive) confirmations.Optionally filter to only include txouts paid to specified addresses.Results are an array of Objects, each of which has txid, vout,scriptPubKey, amount, confirmations
---

### Parameters


`minconf` - numeric

Optional, default=1

The minimum confirmations to filter.

`maxconf` - numeric

Optional, default=9999999

The maximum confirmations to filter.

`addresses` - array

A json array of Zcash addresses to filter.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "listunspent",
"params": [null, null, null],
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


---
title: btc:prioritisetransaction \[POST\] {disallowed}
description: Accepts the transaction into mined blocks at a higher (or lower)priority
---

### Parameters


`txid` - string, required

The transaction id.

`dummy` - numeric, optional

DEPRECATED. For forward compatibility use named arguments and omit this
parameter.

`fee_delta` - numeric, required

The fee value (in satoshis) to add (or subtract, if negative).

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "prioritisetransaction",
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


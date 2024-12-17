---
title: btc:gettxoutsetinfo \[POST\] {disallowed}
description: Returns statistics about the unspent transaction output set.Note this call may take some time.
---

### Parameters


`hash_type` - string, optional, default=hash_serialized_2

Which UTXO set hash should be calculated. Options 'hash_serialized_2'
(thelegacy algorithm), 'none'."

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "gettxoutsetinfo",
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


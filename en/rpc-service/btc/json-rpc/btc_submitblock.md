---
title: btc:submitblock \[POST\] {disallowed}
description: Attempts to submit new block to network.
---

### Parameters


`hexdata` - string, required

the hex-encoded block data to submit

`dummy` - string, optional, default=ignored

Dummy value, for compatibility with BIP22. This value is ignored.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "submitblock",
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


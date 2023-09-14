---
title: doge:listunspent \[POST\] {disallowed}
description: Returns a list of unspent transaction inputs in the wallet.
---

### Parameters


`minconf` - integer

Minimum number of confirmations required to be listed.

`maxconf` - integer

Maximal number of confirmations allowed to be listed.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "listunspent",
"params": [1, 999999],
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


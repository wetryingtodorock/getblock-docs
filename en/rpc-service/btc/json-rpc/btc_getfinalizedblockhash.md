---
title: btc:getfinalizedblockhash \[POST\]
description: Returns the hash of the currently finalized block
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getfinalizedblockhash",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "000000000000000000073da808b05b4b94337d838b3e0a5b98f25b98363216c3"
}
```


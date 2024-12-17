---
title: btc:unparkblock \[POST\] {disallowed}
description: Removes parked status of a block and its descendants, reconsider themfor activation.This can be used to undo the effects of parkblock.
---

### Parameters


`blockhash` - string, required

the hash of the block to unpark

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "unparkblock",
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


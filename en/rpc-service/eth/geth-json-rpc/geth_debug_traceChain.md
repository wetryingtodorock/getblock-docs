---
title: geth:debug_traceChain \[POST\] {disallowed}
description: Returns the structured logs created during the execution of EVM betweentwo blocks (excluding start) as a JSON object. This endpoint must beinvoked via debug_subscribe.
---

### Parameters


`first` - string

hex number of start block

`last` - string

hex number of last block

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_traceChain",
"params": ["0x000DB5cb74A30bbc2F21A3F3DD501E8E0585816a", "0x97a363e191f1f01459b2a9987edd7c01c962f4ce"],
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


---
title: zec:setgenerate  {disallowed} - Zcash
description: Example code for the zec:setgenerate  {disallowed} json-rpc method. Сomplete guide on how to use zec:setgenerate  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`generate` - boolean

Set to true to turn on generation, off to turn off.

`genproclimit` - limit

Optional

Set the processor limit for when generation is on. Can be -1 for
unlimited.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "setgenerate",
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


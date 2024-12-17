---
title: logging  {disallowed} - Bitcoin
description: Example code for the logging  {disallowed} json-rpc method. Сomplete guide on how to use logging  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`include` - json array, optional

A json array of categories to add debug logging

`exclude` - json array, optional

A json array of categories to remove debug logging

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "logging",
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


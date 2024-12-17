---
title: btc:importmulti  {disallowed} - Bitcoin
description: Example code for the btc:importmulti  {disallowed} json-rpc method. Сomplete guide on how to use btc:importmulti  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`requests` - json array, required

Data to be imported

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "importmulti",
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


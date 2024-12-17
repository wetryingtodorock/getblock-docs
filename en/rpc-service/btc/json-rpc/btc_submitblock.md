---
title: btc:submitblock  {disallowed} - Bitcoin
description: Example code for the btc:submitblock  {disallowed} json-rpc method. Сomplete guide on how to use btc:submitblock  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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


---
title: bch:verifychain  {disallowed} - Bitcoin Cash
description: Example code for the bch:verifychain  {disallowed} json-rpc method. Сomplete guide on how to use bch:verifychain  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`checklevel` - numeric, optional, default=3, range=0-4

How thorough the block verification

`nblocks` - numeric, optional, default=6, 0=all

The number of blocks to check.

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "verifychain",
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


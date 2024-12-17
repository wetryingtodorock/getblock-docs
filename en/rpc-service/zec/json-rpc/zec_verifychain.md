---
title: zec:verifychain  {disallowed} - Zcash
description: Example code for the zec:verifychain  {disallowed} json-rpc method. Сomplete guide on how to use zec:verifychain  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`checklevel` - numeric

Optional.

0-4, default=3

How thorough the block verification is.

`numblocks` - numeric

Optional.

default=288, 0=all

The number of blocks to check.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
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


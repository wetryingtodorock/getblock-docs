---
title: zec:getreceivedbyaccount  {disallowed} - Zcash
description: Example code for the zec:getreceivedbyaccount  {disallowed} json-rpc method. Сomplete guide on how to use zec:getreceivedbyaccount  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`account` - string

Optional.

DEPRECATED. If provided, it MUST be set to the empty string "" or to the
string "\*", either of which will give the total available balance.
Passing any other string will result in an error.

`minconf` - numeric,

Optional, default=1

Only include transactions confirmed at least this many times.

`inZat` - boolean

Optional, default=false

Get the result amount in zatoshis (as an integer).

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getreceivedbyaccount",
"params": [null, null, null],
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


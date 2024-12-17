---
title: bch:getreceivedbyaddress  {disallowed} - Bitcoin Cash
description: Example code for the bch:getreceivedbyaddress  {disallowed} json-rpc method. Сomplete guide on how to use bch:getreceivedbyaddress  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`address` - string, required

The bitcoin address for transactions.

`minconf` - numeric, optional, default=1

Only include transactions confirmed at least this many times.

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getreceivedbyaddress",
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


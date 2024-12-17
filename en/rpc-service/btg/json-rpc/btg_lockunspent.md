---
title: btg:lockunspent  {disallowed} - Bitcoin Gold
description: Example code for the btg:lockunspent  {disallowed} json-rpc method. Сomplete guide on how to use btg:lockunspent  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`unlock` - boolean, required

Whether to unlock (true) or lock (false) the specified transactions

`transactions` - json array, optional, default=empty array

The transaction outputs and within each, the txid (string) vout
(numeric).

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "lockunspent",
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


---
title: importprivkey  {disallowed} - Zcash
description: Example code for the importprivkey  {disallowed} json-rpc method. Сomplete guide on how to use importprivkey  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`zcashprivkey` - string

The private key.

`label` - string

Optional, default=""

An optional label.

`rescan` - boolean

Optional, default=false

Rescan the wallet for transactions.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "importprivkey",
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

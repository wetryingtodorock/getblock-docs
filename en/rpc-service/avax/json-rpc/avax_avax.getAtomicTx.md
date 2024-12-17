---
title: avax:avax.getAtomicTx \[POST\] {disallowed}
description: Gets a transaction by its ID.
---

### Parameters


`txID` - string

txID is the transacion ID. It should be in cb58 format.

`encoding` - string

Optional encoding parameter to specify the format for the returned
transaction. Can be either cb58 or hex. Defaults to cb58.

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "avax.getAtomicTx",
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


---
title: dash:importprunedfunds \[POST\] {disallowed}
description: imports funds without the need of a rescan. Meant for use with prunedwallets. Corresponding address or script must previously be included inwallet.The end-user is responsible to import additional transactions thatsubsequently spend the imported outputs or rescan after the point in theblockchain the transaction is included.
---

### Parameters


`Raw Transaction` - string (hex)

A raw transaction in hex funding an already-existing address in wallet.

`TX Out Proof` - string (hex)

The hex output from gettxoutproof that contains the transaction.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "importprunedfunds",
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


---
title: btg:importprunedfunds \[POST\] {disallowed}
description: Imports funds without rescan. Corresponding address or script mustpreviously be included in wallet. Aimed towards pruned wallets. Theend-user is responsible to import additional transactions thatsubsequently spend the imported outputs or rescan after the point in theblockchain the transaction is included.
---

### Parameters


`rawtransaction` - string, required

A raw transaction in hex funding an already-existing address in wallet

`txoutproof` - string, required

The hex output from gettxoutproof that contains the transaction

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
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


---
title: zec:fundrawtransaction \[POST\]
description: Add inputs to a transaction until it has enough in value to meet its outvalue.This will not modify existing inputs, and will add one change output tothe outputs.Note that inputs which were signed may need to be resigned aftercompletion since in/outputs have been added.The inputs added will not be signed, use signrawtransaction for that.Note that all existing inputs must have their previous outputtransaction be in the wallet.Note that all inputs selected must be of standard form and P2SH scriptsmust bein the wallet using importaddress or addmultisigaddress (tocalculate fees).Only pay-to-pubkey, multisig, and P2SH versions thereof are currentlysupported for watch-only
---

### Parameters


`hexstring` - string

The hex string of the raw transaction.

`includeWatching` - boolean

Optional, default=false

Also select inputs which are watch only.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "fundrawtransaction",
"params": [null, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": null
}
```


---
title: btg:importmulti \[POST\] {disallowed}
description: Import addresses/scripts (with private or public keys, redeem script(P2SH)), optionally rescanning the blockchain from the earliest creationtime of the imported scripts. Requires a new wallet backup.If an address/script is imported without all of the private keysrequired to spend from that address, it will be watchonly. The‘watchonly’ option must be set to true in this case or a warning will bereturned.Conversely, if all the private keys are provided and the address/scriptis spendable, the watchonly option must be set to false, or a warningwill be returned.Note This call can take over an hour to complete if rescan is true,during that time, other rpc calls may report that the imported keys,addresses or scripts exist but related transactions are still missing.Note Use “getwalletinfo” to query the scanning progress.
---

### Parameters


`requests` - json array, required

Data to be imported

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "importmulti",
"params": [null],
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


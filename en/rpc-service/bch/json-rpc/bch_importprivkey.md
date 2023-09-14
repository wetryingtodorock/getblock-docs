---
title: bch:importprivkey \[POST\] {disallowed}
description: Adds a private key (as returned by dumpprivkey) to your wallet. Requiresa new wallet backup.Hint use importmulti to import more than one private key.Note This call can take over an hour to complete if rescan is true,during that time, other rpc calls may report that the imported keyexists but related transactions are still missing, leading totemporarily incorrect/bogus balances and unspent outputs until rescancompletes.Note Use “getwalletinfo” to query the scanning progress.
---

### Parameters


`privkey` - string, required

The private key (see dumpprivkey)

`label` - string, optional, default=current label if address exists,
otherwise “”

An optional label

`rescan` - boolean, optional, default=true

Rescan the wallet for transactions

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
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


---
title: dgb:importpubkey \[POST\] {disallowed}
description: Adds a public key (in hex) that can be watched as if it were in yourwallet but cannot be used to spend. Requires a new wallet backup.Hint use importmulti to import more than one public key.Note This call can take over an hour to complete if rescan is true,during that time, other rpc calls may report that the imported pubkeyexists but related transactions are still missing, leading totemporarily incorrect/bogus balances and unspent outputs until rescancompletes.Note Use “getwalletinfo” to query the scanning progress.
---

### Parameters


`pubkey` - string, required

The hex-encoded public key

`label` - string, optional, default=””

An optional label

`rescan` - boolean, optional, default=true

Rescan the wallet for transactions

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "importpubkey",
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


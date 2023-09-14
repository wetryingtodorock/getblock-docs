---
title: dgb:importaddress \[POST\] {disallowed}
description: Adds an address or script (in hex) that can be watched as if it were inyour wallet but cannot be used to spend. Requires a new wallet backup.Note This call can take over an hour to complete if rescan is true,during that time, other rpc calls may report that the imported addressexists but related transactions are still missing, leading totemporarily incorrect/bogus balances and unspent outputs until rescancompletes.If you have the full public key, you should call importpubkey instead ofthis.Hint use importmulti to import more than one address.Note If you import a non-standard raw script in hex form, outputssending to it will be treated as change, and not show up in many RPCs.Note Use “getwalletinfo” to query the scanning progress.
---

### Parameters


`address` - string, required

The Bitcoin address (or hex-encoded script)

`label` - string, optional, default=””

An optional label

`rescan` - boolean, optional, default=true

Rescan the wallet for transactions

`p2sh` - boolean, optional, default=false

Add the P2SH version of the script as well

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "importaddress",
"params": [null, null, null, null],
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


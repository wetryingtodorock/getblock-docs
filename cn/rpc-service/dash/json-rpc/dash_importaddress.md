---
title: dash:importaddress \[POST\] {disallowed}
description: Adds an address or pubkey script to the wallet without the associatedprivate key, allowing you to watch for transactions affecting thataddress or pubkey script without being able to spend any of its outputs.
---

### Parameters


`Address or Script` - string (base58 or hex)

Either a P2PKH or P2SH address encoded in base58check, or a pubkey
script encoded as hex.

`Label` - string

An optional label. Default is an empty string.

`Rescan` - bool

Optional.

Set to true (the default) to rescan the entire local block database for
transactions affecting any address or pubkey script in the wallet
(including transaction affecting the newly-added address or pubkey
script).

Set to false to not rescan the block database (rescanning can be
performed at any time by restarting Dash Core with the -rescan
command-line argument). Rescanning may take several minutes.

`P2SH` - bool

Optional.

Add the P2SH version of the script as well.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
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


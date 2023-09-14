---
title: dash:validateaddress \[POST\]
description: Returns information about the given Dash address.Dash Core 0.17.0 DeprecationsParts of this command have been deprecated and moved to thegetaddressinfo RPC. Clients must transition to using getaddressinfo toaccess this information before upgrading to v0.18.The following deprecated fields have moved to getaddressinfo and willonly be shown here with -deprecatedrpc=validateaddress ismine,iswatchonly, script, hex, pubkeys, sigsrequired, pubkey, addresses,embedded, iscompressed, account, timestamp, hdkeypath.
---

### Parameters


`Address` - string (base58)

The P2PKH or P2SH address to validate encoded in base58check format.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "validateaddress",
"params": ["7n9YufoWBrJ65YC7sgwk53EzbPHMQRB6HJ"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "address": "7n9YufoWBrJ65YC7sgwk53EzbPHMQRB6HJ",
        "isscript": true,
        "isvalid": true,
        "scriptPubKey": "a914d887657080297c7ee1d2faf3970017c82bdf8b5487"
    }
}
```


---
title: btg:addmultisigaddress \[POST\] {disallowed}
description: Add an nrequired-to-sign multisignature address to the wallet. Requiresa new wallet backup.Each key is a Bitcoin address or hex-encoded public key.This functionality is only intended for use with non-watchonly addressesSee \`importaddress\` for watchonly p2sh address support.If label is specified, assign address to that label.
---

### Parameters


`nrequired` - numeric, required

The number of required signatures out of the n keys or addresses.

`keys` - json array, required

The bitcoin addresses or hex-encoded public keys

`label` - string, optional

A label to assign the addresses to.

`address_type` - string, optional

A label to assign the addresses to.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "addmultisigaddress",
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


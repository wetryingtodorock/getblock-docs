---
title: bch:importpubkey  {disallowed} - Bitcoin Cash
description: Example code for the bch:importpubkey  {disallowed} json-rpc method. Сomplete guide on how to use bch:importpubkey  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
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


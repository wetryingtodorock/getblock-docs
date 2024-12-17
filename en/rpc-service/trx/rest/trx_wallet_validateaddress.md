---
title: trx:/wallet/validateaddress \[POST\]
description: Validates address, returns either true or false.
---

### Parameters


`address` - string

Address should be in base58checksum, hexString, or base64 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/validateaddress' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"address": "4189139CB1387AF85E3D24E212A008AC974967E561"}'
```

###  Response

``` java
{
    "message": "Hex string format",
    "result": true
}
```


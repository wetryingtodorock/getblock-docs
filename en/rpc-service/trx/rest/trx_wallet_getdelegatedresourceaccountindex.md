---
title: /wallet/getdelegatedresourceaccountindex  {disallowed} - TRON
description: Example code for the /wallet/getdelegatedresourceaccountindex  {disallowed} rest method. Сomplete guide on how to use /wallet/getdelegatedresourceaccountindex  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`value` - string

Address, default hexString

`visible` - boolean

Optional. Defaults to false. Whether addresses are in base58check
format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getdelegatedresourceaccountindex' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"value": "4189139CB1387AF85E3D24E212A008AC974967E561"}'
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


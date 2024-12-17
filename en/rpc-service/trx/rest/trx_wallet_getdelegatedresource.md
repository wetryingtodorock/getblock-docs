---
title: trx:/wallet/getdelegatedresource \[POST\] {disallowed}
description: Returns all resources delegations from an account to another account.The fromAddress can be retrieved from theGetDelegatedResourceAccountIndex API.
---

### Parameters


`fromAddress` - string, required

Energy from address, default hexString

`toAddress` - string, required

Energy delegation information

`visible` - boolean

Optional. Defaults to false. Whether addresses are in base58check
format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getdelegatedresource' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"fromAddress": "4189139CB1387AF85E3D24E212A008AC974967E561", "toAddress": "41af80f3c6d502b0f53e5fdd2d09d52051a3ba7054"}'
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


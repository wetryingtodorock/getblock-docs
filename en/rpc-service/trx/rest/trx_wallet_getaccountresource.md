---
title: trx:/wallet/getaccountresource \[POST\] {disallowed}
description: Query the resource information of an account (bandwidth, energy, etc)
---

### Parameters


`address` - string

Address:default hexString

`visible` - boolean

Optional,whether the address is in base58 format

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getaccountresource' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{}'
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


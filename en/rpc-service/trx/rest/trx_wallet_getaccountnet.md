---
title: trx:/wallet/getaccountnet  {disallowed} - TRON
description: Example code for the trx:/wallet/getaccountnet  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/getaccountnet  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`address` - string

Address:default hexString

`visible` - boolean

Optional,whether the address is in base58 format

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getaccountnet' \
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


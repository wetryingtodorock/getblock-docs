---
title: trx:/wallet/getassetissuebyaccount  {disallowed} - TRON
description: Example code for the trx:/wallet/getassetissuebyaccount  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/getassetissuebyaccount  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`address` - string

Address is the Token Issuer account address

`visible` - boolean

Optional. Defaults to false. Whether addresses are in base58check
format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getassetissuebyaccount' \
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


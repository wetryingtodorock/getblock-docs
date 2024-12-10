---
title: trx:/wallet/getaccount  {disallowed} - TRON
description: Example code for the trx:/wallet/getaccount  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/getaccount  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`address` -

string

address should be converted to a hex string

`visible` -

string

Optional,whether the address is in base58 format

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getaccount' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"address": "some address"}'
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


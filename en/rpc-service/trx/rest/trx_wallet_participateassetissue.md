---
title: trx:/wallet/participateassetissue  {disallowed} - TRON
description: Example code for the trx:/wallet/participateassetissue  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/participateassetissue  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`to_address` - string

`owner_address` - string

The participant address, default hexString

`amount` - int64

The number of trx participating in token issuance

`asset_name` - string

Token id, default hexString

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/participateassetissue' \
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


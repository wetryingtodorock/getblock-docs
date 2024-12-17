---
title: /wallet/easytransferassetbyprivate  {disallowed} - TRON
description: Example code for the /wallet/easytransferassetbyprivate  {disallowed} rest method. Сomplete guide on how to use /wallet/easytransferassetbyprivate  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`privateKey` - string

Private key, default hexString

`toAddress` - string

To address, default hexString

`assetid` - string

Token id

`amount` - int64

Transfer token amount,the unit is the smallest unit.

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/easytransferassetbyprivate' \
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


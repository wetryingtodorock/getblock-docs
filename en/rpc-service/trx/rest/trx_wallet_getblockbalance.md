---
title: trx:/wallet/getblockbalance  {disallowed} - TRON
description: Example code for the trx:/wallet/getblockbalance  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/getblockbalance  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`hash` - string

`number` - int32

`visible` - boolean

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getblockbalance' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"hash": "0000000001d6f49f02810b1aeb2dab52cbc72bb269388b9cea453a6fd934e7fd"}'
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


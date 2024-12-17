---
title: trx:/wallet/getpaginatedassetissuelist  {disallowed} - TRON
description: Example code for the trx:/wallet/getpaginatedassetissuelist  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/getpaginatedassetissuelist  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`offset` - int32

The index of the start token

`limit` - int32

The amount of tokens per page

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getpaginatedassetissuelist' \
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


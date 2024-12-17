---
title: trx:/walletsolidity/gettransactionbyid \[POST\] {disallowed}
description: Get solidity transaction by its ID
---

### Parameters


`value` - string

transaction ID.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/walletsolidity/gettransactionbyid' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"value": "d78f3db7dbdacd656ddf5ccbe4fac4d6012a979cbdbbaa817a1bdd04ce9f5d02"}'
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


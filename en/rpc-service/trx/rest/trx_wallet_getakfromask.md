---
title: trx:/wallet/getakfromask \[POST\] {disallowed}
description: Note To ensure security, Trongrid has disabled this interface service,please use the service provided by the local node.
---

### Parameters


`value` - string, required

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getakfromask' \
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


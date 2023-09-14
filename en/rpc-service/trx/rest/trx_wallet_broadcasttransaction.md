---
title: trx:/wallet/broadcasttransaction \[POST\] {disallowed}
description: Broadcast the signed transaction
---

### Parameters


`txID` - string

`visible` - boolean

`raw_data` - json object

`raw_data_hex` - string

`signature` - array of string

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/broadcasttransaction' \
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


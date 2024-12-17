---
title: trx:/wallet/getpaginatedassetissuelist \[POST\] {disallowed}
description: Query the list of all the tokens by pagination.Returns a list of Tokensthat succeed the Token located at offset.
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


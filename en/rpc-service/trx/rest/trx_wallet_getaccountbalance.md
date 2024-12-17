---
title: trx:/wallet/getaccountbalance \[POST\] {disallowed}
description: Get the account balance in a specific block. (Note At present, theinterface data can only be queried through the following official nodes47.241.20.47, 161.117.85.97, 161.117.224.116, 161.117.83.38)
---

### Parameters


`account_identifier` - json object

`block_identifier` - json object

`visible` - boolean

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getaccountbalance' \
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


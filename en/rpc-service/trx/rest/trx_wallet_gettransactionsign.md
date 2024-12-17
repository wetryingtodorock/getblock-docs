---
title: trx:/wallet/gettransactionsign \[POST\] {disallowed}
description: Sign the transaction, the api has the risk of leaking the private key,please make sure to call the api in a secure environment
---

### Parameters


`transaction` - json object

Transaction is a contract created by http api

Format: - txID - string - visible - boolean - raw_data - json object -
raw_data_hex - string - signature - array of string

`privateKey` - string

privateKey is the user private key

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/gettransactionsign' \
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


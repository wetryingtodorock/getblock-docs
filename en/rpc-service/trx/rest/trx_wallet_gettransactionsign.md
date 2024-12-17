---
title: /wallet/gettransactionsign  {disallowed} - TRON
description: Example code for the /wallet/gettransactionsign  {disallowed} rest method. Сomplete guide on how to use /wallet/gettransactionsign  {disallowed} rest in GetBlock.io Web3 documentation.
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


---
title: /wallet/broadcasttransaction - TRON
description: Example code for the /wallet/broadcasttransaction rest method. Сomplete guide on how to use /wallet/broadcasttransaction rest in GetBlock.io Web3 documentation.
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


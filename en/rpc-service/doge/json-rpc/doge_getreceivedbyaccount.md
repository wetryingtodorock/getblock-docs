---
title: doge:getreceivedbyaccount \[POST\] {disallowed}
description: Returns the total amount received by addresses with an account intransactions with at least a certain number of confirmations.
---

### Parameters


`account` - string

Account to query for total amount.

`minconf` - integer

Number of confirmations to require, defaults to 1.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getreceivedbyaccount",
"params": [null, 1],
"id": "getblock.io"}'
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


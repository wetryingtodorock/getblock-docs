---
title: doge:getreceivedbyaddress \[POST\] {disallowed}
description: Returns the total amount received by a dogecoin address in transactionswith at least a certain number of confirmations.
---

### Parameters


`dogecoinaddress` - string

Address to query for total amount.

`minconf` - integer

Number of confirmations to require, defaults to 1.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getreceivedbyaddress",
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


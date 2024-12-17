---
title: etc:priv_getLogs \[POST\] {disallowed}
description: Returns an array of logs matching a specified filter object.For private contracts, priv_getLogs is the same as eth_getLogs forpublic contracts except there is no automatic log bloom caching forprivate contracts.
---

### Parameters


`data` - None

32-byte privacy Group ID.

`Object` - None

Filter options object.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_getLogs",
"params": [null, null],
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


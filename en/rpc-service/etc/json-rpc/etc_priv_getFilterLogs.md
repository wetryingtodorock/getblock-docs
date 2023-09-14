---
title: etc:priv_getFilterLogs \[POST\] {disallowed}
description: Returns an array of logs for the specified filter for a privatecontract.For private contracts, priv_getFilterLogs is the same aseth_getFilterLogs for public contracts except there is no automatic logbloom caching for private contracts.
---

### Parameters


`data` - None

32-byte privacy Group ID.

`data` - None

Filter ID.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_getFilterLogs",
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


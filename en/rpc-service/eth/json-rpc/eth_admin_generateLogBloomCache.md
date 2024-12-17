---
title: eth:admin_generateLogBloomCache \[POST\] {disallowed}
description: Generates cached log bloom indexes for blocks. APIs such as eth_getLogsand eth_getFilterLogs use the cache for improved performance.
---

### Parameters


`integer` - None

Block to start generating indexes.

`integer` - None

Block to start generating indexes.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "admin_generateLogBloomCache",
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


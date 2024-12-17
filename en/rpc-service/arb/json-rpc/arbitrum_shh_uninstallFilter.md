---
title: arbitrum:shh_uninstallFilter \[POST\] {disallowed}
description: Uninstalls a filter with given id. Should always be called when watch isno longer needed.Additonally Filters timeout when they aren’t requested withshh_getFilterChanges for a period of time.
---

### Parameters


`id` - string

the filter id.

### Request

``` java
curl --location --request POST 'https://arbitrum.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "shh_uninstallFilter",
"params": [null],
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


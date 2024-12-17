---
title: gno:eth_uninstallFilter \[POST\]
description: Uninstalls a filter with the specified ID. When a filter is no longerrequired, call this method.Filters time out when not requested by eth_getFilterChanges oreth_getFilterLogs for 10 minutes.
---

### Parameters


`data` - hex string

Filter ID.

### Request

``` java
curl --location --request POST 'https://gno.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_uninstallFilter",
"params": ["0x6b08"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": true
}
```


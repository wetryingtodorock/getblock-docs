---
title: kcc:eth_uninstallFilter \[POST\]
description: Uninstalls a filter with given id. Should always be called when watch isno longer needed. Additonally Filters timeout when they aren’t requestedwith eth_getFilterChanges for a period of time.
---

### Parameters


`QUANTITY` - string

The filter id.

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_uninstallFilter",
"params": ["0x17d41b42a97cd7bf3c77c25a79c49c88"],
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


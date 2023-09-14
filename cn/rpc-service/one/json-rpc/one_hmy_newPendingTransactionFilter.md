---
title: one:hmy_newPendingTransactionFilter \[POST\]
description: Creates a filter in the node, to notify when new pending transactionsarrive. To check if the state has changed, call hmy_getFilterChanges.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://one.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "hmy_newPendingTransactionFilter",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x4d09fd774f646f97b08c50662d1ddb1f"
}
```


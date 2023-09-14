---
title: optimism:eth_newPendingTransactionFilter \[POST\]
description: Creates a filter in the node, to notify when new pending transactionsarrive. To check if the state has changed, call eth_getFilterChanges.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newPendingTransactionFilter",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xc1174f6beddcf45dd8dfa305f4b8eeca"
}
```


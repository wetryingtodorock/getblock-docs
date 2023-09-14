---
title: etc:eth_newPendingTransactionFilter \[POST\]
description: Creates a filter to retrieve new pending transactions hashes. To pollfor new pending transactions, use eth_getFilterChanges.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
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
    "result": "0x8541af777b207ffd5ca2f9577fd6af92"
}
```


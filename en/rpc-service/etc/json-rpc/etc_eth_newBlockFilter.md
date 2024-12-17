---
title: etc:eth_newBlockFilter \[POST\]
description: Creates a filter to retrieve new block hashes. To poll for new blocks,use eth_getFilterChanges.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newBlockFilter",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xf316534bea726e1bf51b4ea4f3bad48d"
}
```


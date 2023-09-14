---
title: one:hmy_newBlockFilter \[POST\]
description: Creates a filter in the node, to notify when a new block arrives. Tocheck if the state has changed, call hmy_getFilterChanges.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://one.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "hmy_newBlockFilter",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xa61ae00341ddec46a6a165f0fd65d110"
}
```


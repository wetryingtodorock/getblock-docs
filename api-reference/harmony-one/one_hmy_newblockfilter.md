---
title: hmy_newBlockFilter - Harmony
description: Example code for the hmy_newBlockFilter json-rpc method. Сomplete guide on how to use hmy_newBlockFilter json-rpc in GetBlock.io Web3 documentation.
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


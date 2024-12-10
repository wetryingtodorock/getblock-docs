---
title: dgb:getdifficulty - DigiByte
description: Example code for the dgb:getdifficulty json-rpc method. Сomplete guide on how to use dgb:getdifficulty json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getdifficulty",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": 111625.4745815573
}
```


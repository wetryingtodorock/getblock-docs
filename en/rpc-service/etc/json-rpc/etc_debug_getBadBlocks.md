---
title: etc:debug_getBadBlocks  {disallowed} - Ethereum Classic
description: Example code for the etc:debug_getBadBlocks  {disallowed} json-rpc method. Сomplete guide on how to use etc:debug_getBadBlocks  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "debug_getBadBlocks",
"params": [],
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


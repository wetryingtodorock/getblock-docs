---
title: dash:getmininginfo - Dash
description: Example code for the dash:getmininginfo json-rpc method. Сomplete guide on how to use dash:getmininginfo json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getmininginfo",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "blocks": 1535914,
        "chain": "main",
        "currentblocksize": 3921,
        "currentblocktx": 9,
        "difficulty": 103704145.924301,
        "networkhashps": 2972518180727094,
        "pooledtx": 7,
        "warnings": ""
    }
}
```


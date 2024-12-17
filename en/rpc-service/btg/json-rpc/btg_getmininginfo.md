---
title: btg:getmininginfo - Bitcoin Gold
description: Example code for the btg:getmininginfo json-rpc method. Сomplete guide on how to use btg:getmininginfo json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
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
        "blocks": 702634,
        "chain": "main",
        "currentblocktx": 0,
        "currentblockweight": 4000,
        "difficulty": 197682.9725910754,
        "networkhashps": 2324661.797680737,
        "pooledtx": 0,
        "warnings": ""
    }
}
```


---
title: doge:getmininginfo \[POST\]
description: Returns an MiningInfo object containing various mining state info.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
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
        "blocks": 3906176,
        "chain": "main",
        "currentblocksize": 0,
        "currentblocktx": 0,
        "currentblockweight": 0,
        "difficulty": 4386136.832791463,
        "errors": "",
        "networkhashps": 301649146285387.1,
        "pooledtx": 32
    }
}
```


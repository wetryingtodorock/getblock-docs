---
title: dash:getbestblockhash \[POST\]
description: Returns the header hash of the most recent block on the best blockchain.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getbestblockhash",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "0000000000000019cd3a50eedc418372f7aa9060d6ded56a769a51a93dfe0e4a"
}
```


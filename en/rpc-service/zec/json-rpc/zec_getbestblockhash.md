---
title: zec:getbestblockhash \[POST\]
description: Returns the hash of the best (tip) block in the longest block chain.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
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
    "result": "00000000019af1612080b8d6b3ce87c5b7569a114e6a77385260cf45a6419fe1"
}
```


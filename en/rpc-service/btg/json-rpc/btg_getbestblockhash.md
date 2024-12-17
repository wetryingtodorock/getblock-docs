---
title: btg:getbestblockhash \[POST\]
description: Returns the hash of the best (tip) block in the most-workfully-validated chain.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
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
    "result": "000000007cc1fc836d0992202730ca71f77a8cf2a35974ca300dadbf8bc1e090"
}
```


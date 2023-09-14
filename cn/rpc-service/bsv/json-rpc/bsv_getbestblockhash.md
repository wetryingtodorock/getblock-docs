---
title: bsv:getbestblockhash \[POST\]
description: Returns the hash of the best (tip) block in the most-workfully-validated chain.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
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
    "result": "0000000000000000023a561e1ea370153aac5d1504726d1a039032831c05fcfc"
}
```


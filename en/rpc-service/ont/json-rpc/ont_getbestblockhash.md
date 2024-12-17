---
title: ont:getbestblockhash \[POST\]
description: Fetch block hash for the highest block for the current node.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ont.getblock.io/mainnet/' 
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
    "desc": "SUCCESS",
    "error": 0,
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "449822980132ae033acf72fd5530db33a3963964d51c7ce81fe3aadb763a50b4"
}
```


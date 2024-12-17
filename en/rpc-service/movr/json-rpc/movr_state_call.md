---
title: movr:state_call \[POST\] {disallowed}
description: Perform a call to a builtin on the chain.
---

### Parameters


`method` - Text

method to call

`data` - Bytes

data

`at` - BlockHash

block hash

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "state_call",
"params": [null, null, null],
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


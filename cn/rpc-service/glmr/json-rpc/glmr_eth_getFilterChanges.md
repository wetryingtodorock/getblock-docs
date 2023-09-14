---
title: glmr:eth_getFilterChanges \[POST\]
description: Polling method for a filter, which returns an array of logs whichoccurred since last poll.
---

### Parameters


`QUANTITY` - string

The filter id.

### Request

``` java
curl --location --request POST 'https://glmr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getFilterChanges",
"params": ["0x16"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32603,
        "message": "Filter id 22 does not exist."
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```


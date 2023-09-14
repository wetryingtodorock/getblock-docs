---
title: gno:eth_getFilterLogs \[POST\]
description: Returns an array of logs for the specified filter.Leave the --auto-log-bloom-caching-enabled command line option at thedefault value of true to improve log retrieval performance.
---

### Parameters


`data` - None

Filter ID.

### Request

``` java
curl --location --request POST 'https://gno.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getFilterLogs",
"params": ["0x5ace5de3985749b6a1b2b0d3f3e1fb69"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32603,
        "message": "Filter with id: '120702037069533879537037142191838985065' does not exist."
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```


---
title: etc:eth_newFilter \[POST\]
description: Creates a log filter. To poll for logs associated with the createdfilter, use eth_getFilterChanges. To get all logs associated with thefilter, use eth_getFilterLogs.
---

### Parameters


`Object` - None

Filter options object.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newFilter",
"params": [{"fromBlock": "earliest", "toBlock": "latest", "topics": []}],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x3df538d9a3093afae00756ee16412677"
}
```


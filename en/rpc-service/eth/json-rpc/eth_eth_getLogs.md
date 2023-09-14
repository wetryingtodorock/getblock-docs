---
title: eth:eth_getLogs \[POST\]
description: Returns an array of logs matching a specified filter object.Leave the --auto-log-bloom-caching-enabled command line option at thedefault value of true to improve log retrieval performance.
---

### Parameters


`Object` - None

Filter options object.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getLogs",
"params": [{"fromBlock": "0x107D7B0", "toBlock": "0x107D7B0", "address": "0x901c7C311d39e0b26257219765E71E8DB3107A81", "topics": []}],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": []
}
```


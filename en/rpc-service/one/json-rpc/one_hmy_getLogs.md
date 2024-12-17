---
title: one:hmy_getLogs \[POST\]
description: Returns an array of logs matching a specified filter object.Leave the --auto-log-bloom-caching-enabled command line option at thedefault value of true to improve log retrieval performance.
---

### Parameters


`Object` - hex string

Filter options object.

### Request

``` java
curl --location --request POST 'https://one.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "hmy_getLogs",
"params": [{"fromBlock": "0x8252EC", "toBlock": "0x8252EC", "address": "0x227f6757289a86c13eee2e91c2e6eb03f2ed11a6", "topics": []}],
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


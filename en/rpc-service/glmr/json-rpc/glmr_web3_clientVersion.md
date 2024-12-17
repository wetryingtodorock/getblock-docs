---
title: glmr:web3_clientVersion \[POST\]
description: Returns the current client version.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://glmr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "web3_clientVersion",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "moonbeam/v2302.0/fc-rpc-2.0.0-dev"
}
```


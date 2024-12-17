---
title: heco:web3_clientVersion \[POST\]
description: Returns the current client version.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://heco.getblock.io/mainnet/' 
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
    "result": "Geth/v1.2.2-stable-b07a7152/linux-amd64/go1.19.3"
}
```


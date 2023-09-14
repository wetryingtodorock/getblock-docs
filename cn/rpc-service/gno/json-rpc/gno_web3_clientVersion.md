---
title: gno:web3_clientVersion \[POST\]
description: Returns the current client version.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://gno.getblock.io/mainnet/' 
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
    "result": "Nethermind/v1.18.2+22c00906/linux-x64/dotnet7.0.5"
}
```


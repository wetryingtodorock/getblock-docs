---
title: movr:chain_getFinalizedHead - Moonriver
description: Example code for the movr:chain_getFinalizedHead json-rpc method. Сomplete guide on how to use movr:chain_getFinalizedHead json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "chain_getFinalizedHead",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x32dc93cb9c89a0fe0a4486cd9c05ebdeee4d8d9324c7612cc120b4728f6c3bb6"
}
```


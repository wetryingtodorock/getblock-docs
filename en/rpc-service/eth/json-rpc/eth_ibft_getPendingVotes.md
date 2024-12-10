---
title: eth:ibft_getPendingVotes  {disallowed} - Ethereum
description: Example code for the eth:ibft_getPendingVotes  {disallowed} json-rpc method. Сomplete guide on how to use eth:ibft_getPendingVotes  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "ibft_getPendingVotes",
"params": [],
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


---
title: dot:chain_subscribeAllHeads  {disallowed} - Polkadot
description: Example code for the dot:chain_subscribeAllHeads  {disallowed} json-rpc method. Сomplete guide on how to use dot:chain_subscribeAllHeads  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "chain_subscribeAllHeads",
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


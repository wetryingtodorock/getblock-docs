---
title: dot:eth_newPendingTransactionFilter  {disallowed} - Polkadot
description: Example code for the dot:eth_newPendingTransactionFilter  {disallowed} json-rpc method. Сomplete guide on how to use dot:eth_newPendingTransactionFilter  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newPendingTransactionFilter",
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


---
title: perm_getNodesAllowlist  {disallowed} - Ethereum Classic
description: Example code for the perm_getNodesAllowlist  {disallowed} json-rpc method. Сomplete guide on how to use perm_getNodesAllowlist  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "perm_getNodesAllowlist",
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


---
title: perm_removeNodesFromAllowlist  {disallowed} - Ethereum Classic
description: Example code for the perm_removeNodesFromAllowlist  {disallowed} json-rpc method. Сomplete guide on how to use perm_removeNodesFromAllowlist  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`list of strings` - None

List of enode URLs

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "perm_removeNodesFromAllowlist",
"params": [null],
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

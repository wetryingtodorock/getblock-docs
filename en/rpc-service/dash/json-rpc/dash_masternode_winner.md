---
title: masternode_winner  {disallowed} - Dash
description: Example code for the masternode_winner  {disallowed} json-rpc method. Сomplete guide on how to use masternode_winner  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`method name` - string

None

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "masternode",
"params": ["winner"],
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


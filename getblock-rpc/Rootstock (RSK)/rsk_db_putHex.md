---
title: db_putHex  {disallowed} - Rootstock
description: Example code for the db_putHex  {disallowed} json-rpc method. Сomplete guide on how to use db_putHex  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "db_putHex",
"params": [],
"id": "getblock.io"}
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

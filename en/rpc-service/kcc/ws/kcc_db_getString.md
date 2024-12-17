---
title: kcc:db_getString  {disallowed} - KuCoin Community Chain
description: Example code for the kcc:db_getString  {disallowed} ws method. Сomplete guide on how to use kcc:db_getString  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`database` - string

database name

`key` - string

key name

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "db_getString",
"params": [null, null],
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


---
title: db_putString  {disallowed} - Optimism
description: Example code for the db_putString  {disallowed} ws method. Сomplete guide on how to use db_putString  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`database` - string

database name

`key` - string

key name

`string` - string

string to store.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "db_putString",
"params": [null, null, null],
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


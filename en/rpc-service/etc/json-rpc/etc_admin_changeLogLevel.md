---
title: etc:admin_changeLogLevel  {disallowed} - Ethereum Classic
description: Example code for the etc:admin_changeLogLevel  {disallowed} json-rpc method. Сomplete guide on how to use etc:admin_changeLogLevel  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`level` - None

Log level

`log_filter` - Array

Packages or classes to change the log level for. Optional.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "admin_changeLogLevel",
"params": ["DEBUG", null],
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


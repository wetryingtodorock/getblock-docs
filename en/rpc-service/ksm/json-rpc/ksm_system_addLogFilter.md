---
title: ksm:system_addLogFilter  {disallowed} - Kusama
description: Example code for the ksm:system_addLogFilter  {disallowed} json-rpc method. Сomplete guide on how to use ksm:system_addLogFilter  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`directives` - Text

None

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "system_addLogFilter",
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


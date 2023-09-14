---
title: etc:miner_changeTargetGasLimit \[POST\] {disallowed}
description: Updates the target gas limit set using the --target-gas-limit commandline option.
---

### Parameters


`quantity` - integer

The target gas price in Wei.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "miner_changeTargetGasLimit",
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


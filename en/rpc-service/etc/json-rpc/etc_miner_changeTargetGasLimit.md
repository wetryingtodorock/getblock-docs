---
title: etc:miner_changeTargetGasLimit  {disallowed} - Ethereum Classic
description: Example code for the etc:miner_changeTargetGasLimit  {disallowed} json-rpc method. Сomplete guide on how to use etc:miner_changeTargetGasLimit  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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


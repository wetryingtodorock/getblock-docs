---
title: etc:admin_generateLogBloomCache  {disallowed} - Ethereum Classic
description: Example code for the etc:admin_generateLogBloomCache  {disallowed} json-rpc method. Сomplete guide on how to use etc:admin_generateLogBloomCache  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`integer` - None

Block to start generating indexes.

`integer` - None

Block to start generating indexes.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "admin_generateLogBloomCache",
"params": [null, null],
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


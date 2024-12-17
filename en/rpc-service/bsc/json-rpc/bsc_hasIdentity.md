---
title: hasIdentity  {disallowed} - Binance Smart Chain
description: Example code for the hasIdentity  {disallowed} json-rpc method. Сomplete guide on how to use hasIdentity  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - None

60 Bytes - The identity address to check.

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "hasIdentity",
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


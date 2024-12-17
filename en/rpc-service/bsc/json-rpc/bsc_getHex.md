---
title: getHex  {disallowed} - Binance Smart Chain
description: Example code for the getHex  {disallowed} json-rpc method. Сomplete guide on how to use getHex  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`String` - None

Database name

`String` - None

Key name

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getHex",
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


---
title: debug_traceTransaction  {disallowed} - Ethereum
description: Example code for the debug_traceTransaction  {disallowed} json-rpc method. Сomplete guide on how to use debug_traceTransaction  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`transactionHash` - data

Transaction hash.

`Object` - None

request options (all optional and default to false)

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "debug_traceTransaction",
"params": ["0xcd718a69d478340dc28fdf6bf8056374a52dc95841b44083163ced8dfe29310c", null],
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


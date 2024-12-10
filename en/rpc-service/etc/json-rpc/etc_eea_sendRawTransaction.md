---
title: etc:eea_sendRawTransaction  {disallowed} - Ethereum Classic
description: Example code for the etc:eea_sendRawTransaction  {disallowed} json-rpc method. Сomplete guide on how to use etc:eea_sendRawTransaction  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

Signed RLP-encoded private transaction.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eea_sendRawTransaction",
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


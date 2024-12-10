---
title: zec:signmessage  {disallowed} - Zcash
description: Example code for the zec:signmessage  {disallowed} json-rpc method. Сomplete guide on how to use zec:signmessage  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`t-addr` - string

The transparent address to use for the private key.

`message` - string

The message to create a signature of.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "signmessage",
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


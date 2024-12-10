---
title: cro:eth_sign  {disallowed} - Cronos
description: Example code for the cro:eth_sign  {disallowed} json-rpc method. Сomplete guide on how to use cro:eth_sign  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - hex string

20 Bytes - address

`DATA` - hex string

N Bytes - message to sign

### Request

``` java
curl --location --request POST 'https://cro.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_sign",
"params": ["0x227f6757289a86c13eee2e91c2e6eb03f2ed11a6", "0xbcda"],
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


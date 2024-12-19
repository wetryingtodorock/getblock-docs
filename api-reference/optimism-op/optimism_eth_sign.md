---
title: eth_sign  {disallowed} - Optimism
description: Example code for the eth_sign  {disallowed} json-rpc method. Сomplete guide on how to use eth_sign  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address.

`DATA` - string

message to sign.

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_sign",
"params": ["0xbec4e80531dad6a9989828d174cc2878b1e3123d", "0xdeadbeaf"],
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


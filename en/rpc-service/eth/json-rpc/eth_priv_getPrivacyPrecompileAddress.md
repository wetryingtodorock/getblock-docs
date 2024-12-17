---
title: eth:priv_getPrivacyPrecompileAddress  {disallowed} - Ethereum
description: Example code for the eth:priv_getPrivacyPrecompileAddress  {disallowed} json-rpc method. Сomplete guide on how to use eth:priv_getPrivacyPrecompileAddress  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_getPrivacyPrecompileAddress",
"params": [],
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


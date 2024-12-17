---
title: dot:contracts_upload_code  {disallowed} - Polkadot
description: Example code for the dot:contracts_upload_code  {disallowed} json-rpc method. Сomplete guide on how to use dot:contracts_upload_code  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`uploadRequest` - CodeUploadRequest

None

`at` - BlockHash

optional

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "contracts_upload_code",
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


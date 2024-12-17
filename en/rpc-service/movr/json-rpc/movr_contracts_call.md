---
title: movr:contracts_call  {disallowed} - Moonriver
description: Example code for the movr:contracts_call  {disallowed} json-rpc method. Сomplete guide on how to use movr:contracts_call  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`callRequest` - ContractCallRequest

None

`at` - BlockHash

None

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "contracts_call",
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


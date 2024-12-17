---
title: ksm:web3_sha3  {disallowed} - Kusama
description: Example code for the ksm:web3_sha3  {disallowed} json-rpc method. Сomplete guide on how to use ksm:web3_sha3  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - Bytes

None

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "web3_sha3",
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


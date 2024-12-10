---
title: ksm:eth_getStorageAt  {disallowed} - Kusama
description: Example code for the ksm:eth_getStorageAt  {disallowed} json-rpc method. Сomplete guide on how to use ksm:eth_getStorageAt  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`address` - H160

None

`index` - U256

None

`number` - BlockNumber

None

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getStorageAt",
"params": [null, null, null],
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


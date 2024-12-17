---
title: cro:eth_getBlockReceipts  {disallowed} - Cronos
description: Example code for the cro:eth_getBlockReceipts  {disallowed} json-rpc method. Сomplete guide on how to use cro:eth_getBlockReceipts  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA, 32 Bytes` - None

Block number in hex format or tag.

### Request

``` java
curl --location --request POST 'https://cro.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBlockReceipts",
"params": ["0x8252EC"],
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


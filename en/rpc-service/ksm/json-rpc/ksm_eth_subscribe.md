---
title: ksm:eth_subscribe  {disallowed} - Kusama
description: Example code for the ksm:eth_subscribe  {disallowed} json-rpc method. Сomplete guide on how to use ksm:eth_subscribe  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`kind` - EthSubKind

None

`params` - EthSubParams

None

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_subscribe",
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


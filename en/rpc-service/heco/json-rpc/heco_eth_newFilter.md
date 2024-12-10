---
title: heco:eth_newFilter - Huobi ECO Chain
description: Example code for the heco:eth_newFilter json-rpc method. Сomplete guide on how to use heco:eth_newFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - object

Filter options

### Request

``` java
curl --location --request POST 'https://heco.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newFilter",
"params": [{}],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x7b4662a475efd7d4c22e808a10384464"
}
```


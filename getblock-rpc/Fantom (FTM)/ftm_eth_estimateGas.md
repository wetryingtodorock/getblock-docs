---
title: eth_estimateGas - Fantom
description: Example code for the eth_estimateGas json-rpc method. Сomplete guide on how to use eth_estimateGas json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`object` - object

Transaction call object.

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_estimateGas",
"params": [{"from": "0xFE3B557E8Fb62b89F4916B721be55cEb828dBd73", "to": "0x44Aa93095D6749A706051658B970b941c72c1D53", "value": "0x1"}],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "insufficient balance for transfer"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```


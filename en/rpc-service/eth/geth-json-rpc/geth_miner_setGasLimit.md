---
title: geth:miner_setGasLimit \[POST\] {disallowed}
description: Sets the gas limit the miner will target when mining. Note on networkswhere EIP-1559 is activated, this should be set to twice what you wantthe gas target (i.e. the effective gas used on average per block) to be.
---

### Parameters


`number` - number

gas limit

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "miner_setGasLimit",
"params": [1],
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


---
title: trx:eth_blockNumber - TRON
description: Example code for the trx:eth_blockNumber json-rpc method. Сomplete guide on how to use trx:eth_blockNumber json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/mainnet/jsonrpc' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_blockNumber",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x25ad7ea"
}
```


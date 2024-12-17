---
title: btc:joinpsbts \[POST\]
description: Joins multiple distinct PSBTs with different inputs and outputs into onePSBT with inputs and outputs from all of the PSBTsNo input in any of the PSBTs can be in more than one of the PSBTs.
---

### Parameters


`txs` - json array, required

The base64 strings of partially signed transactions

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "joinpsbts",
"params": [["mybase64_1", "mybase64_2", "mybase64_3"]],
"id": "getblock.io"}'
```


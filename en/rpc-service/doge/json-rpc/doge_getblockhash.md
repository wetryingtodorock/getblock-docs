---
title: doge:getblockhash \[POST\]
description: Returns hash of block in best-block-chain at index.
---

### Parameters


`index` - integer

index of the block.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getblockhash",
"params": [3904788],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "24f64485ea05250ce75a73b3549afad05e078a7d8abd54e695a957dadee264fa"
}
```


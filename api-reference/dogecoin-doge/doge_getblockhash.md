---
title: getblockhash - Dogecoin
description: Example code for the getblockhash json-rpc method. Сomplete guide on how to use getblockhash json-rpc in GetBlock.io Web3 documentation.
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

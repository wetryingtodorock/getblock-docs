---
title: btc:getblockchaininfo \[POST\]
description: Returns an object containing various state info regarding blockchainprocessing.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getblockchaininfo",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "bestblockhash": "0000000000000000023a561e1ea370153aac5d1504726d1a039032831c05fcfc",
        "blocks": 684634,
        "chain": "main",
        "chainwork": "0000000000000000000000000000000000000000016623d7bc4511ec504acf5b",
        "difficulty": 303127737690.0432,
        "headers": 684634,
        "initialblockdownload": false,
        "mediantime": 1619163231,
        "pruned": false,
        "size_on_disk": 183446378110,
        "verificationprogress": 0.9999847435404801,
        "warnings": "Warning: This version of Bitcoin Cash Node is old and may fall out of network consensus in 22 day(s). Please upgrade, or add expire=0 to your configuration file if you want to continue running this version. If you do nothing, the software will gracefully degrade by limiting its functionality in 22 day(s)."
    }
}
```


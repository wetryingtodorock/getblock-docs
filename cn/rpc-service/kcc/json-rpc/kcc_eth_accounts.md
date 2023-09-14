---
title: kcc:eth_accounts \[POST\]
description: Returns a list of addresses owned by client.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_accounts",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        "0x7e5f4552091a69125d5dfcb7b8c2659029395bdf",
        "0x7e5f4552091a69125d5dfcb7b8c2659029395bdf"
    ]
}
```


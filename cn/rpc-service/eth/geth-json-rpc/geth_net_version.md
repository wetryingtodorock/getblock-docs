---
title: geth:net_version \[POST\]
description: Returns the devp2p network ID (e.g. 1 for mainnet, 5 for goerli).
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "net_version",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "1"
}
```


---
title: btc:decodepsbt \[POST\]
description: Return a JSON object representing the serialized, base64-encodedpartially signed Bitcoin transaction.
---

### Parameters


`psbt` - string, required

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "decodepsbt",
"params": ["psbt"],
"id": "getblock.io"}'
```

###  Response

``` java
null
```


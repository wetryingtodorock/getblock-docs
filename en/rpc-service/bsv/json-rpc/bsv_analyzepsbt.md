---
title: bsv:analyzepsbt \[POST\]
description: Analyzes and provides information about the current status of a PSBT andits inputs
---

### Parameters


`psbt` - string, required

A base64 string of a PSBT

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "analyzepsbt",
"params": ["psbt"],
"id": "getblock.io"}'
```


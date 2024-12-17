---
title: bsv:decodescript \[POST\]
description: Decode a hex-encoded script.
---

### Parameters


`hexstring` - string, required

the hex-encoded script

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "decodescript",
"params": ["hexstring"],
"id": "getblock.io"}'
```

###  Response

``` java
null
```


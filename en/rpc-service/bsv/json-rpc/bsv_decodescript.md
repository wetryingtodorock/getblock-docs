---
title: bsv:decodescript - Bitcoin SV
description: Example code for the bsv:decodescript json-rpc method. Сomplete guide on how to use bsv:decodescript json-rpc in GetBlock.io Web3 documentation.
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


---
title: debug_standardTraceBadBlockToFile  {disallowed} - Binance Smart Chain
description: >-
  Example code for the debug_standardTraceBadBlockToFile  {disallowed} json-rpc
  method. Сomplete guide on how to use debug_standardTraceBadBlockToFile 
  {disallowed} json-rpc in GetBlock.io Web3 document
---

# debug\_standardTraceBadBlockToFile  {disallowed} - Binance Smart Chain

#### Parameters

`blockHash` - data

Block hash

#### Request

```java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "debug_standardTraceBadBlockToFile",
"params": ["0x0cf46846c9f2abef8e40ed2f8deea4b789464f44284efe25d443e8d272393fce"],
"id": "getblock.io"}'
```

#### Response

```java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```
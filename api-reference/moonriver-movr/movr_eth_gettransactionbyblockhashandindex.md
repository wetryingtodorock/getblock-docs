---
title: eth_getTransactionByBlockHashAndIndex  {disallowed} - Moonriver
description: >-
  Example code for the eth_getTransactionByBlockHashAndIndex  {disallowed}
  json-rpc method. Сomplete guide on how to use
  eth_getTransactionByBlockHashAndIndex  {disallowed} json-rpc in GetBlock.io
  Web3
---

# eth\_getTransactionByBlockHashAndIndex  {disallowed} - Moonriver

#### Parameters

`hash` - H256

None

`index` - U256

None

#### Request

```java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getTransactionByBlockHashAndIndex",
"params": [null, null],
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

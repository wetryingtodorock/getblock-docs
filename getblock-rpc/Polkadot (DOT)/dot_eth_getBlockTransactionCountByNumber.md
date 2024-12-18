---
title: eth_getBlockTransactionCountByNumber  {disallowed} - Polkadot
description: >-
  Example code for the eth_getBlockTransactionCountByNumber  {disallowed}
  json-rpc method. Сomplete guide on how to use
  eth_getBlockTransactionCountByNumber  {disallowed} json-rpc in GetBlock.io
  Web3 do
---

# eth\_getBlockTransactionCountByNumber  {disallowed} - Polkadot

#### Parameters

`block` - BlockNumber

None

#### Request

```java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByNumber",
"params": [null],
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

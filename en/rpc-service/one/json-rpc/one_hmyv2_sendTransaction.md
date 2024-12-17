---
title: hmyv2_sendTransaction  {disallowed} - Harmony
description: Example code for the hmyv2_sendTransaction  {disallowed} json-rpc method. Сomplete guide on how to use hmyv2_sendTransaction  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - hex string

The transaction object

### Request

``` java
curl --location --request POST 'https://one.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "hmyv2_sendTransaction",
"params": [{"from": "0xb60e8dd61c5d32be8058bb8eb970870f07233155", "to": "0xd46e8dd67c5d32be8058bb8eb970870f07244567", "gas": "0x76c0", "gasPrice": "0x9184e72a000", "value": "0x9184e72a", "data": "0xd46e8dd67c5d32be8d46e8dd67c5d32be8058bb8eb970870f072445675058bb8eb970870f072445675"}],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```


---
title: heco:eth_sendRawTransaction \[POST\]
description: Creates new message call transaction or a contract creation for signedtransactions.
---

### Parameters


`DATA` - string

The signed transaction data.

### Request

``` java
curl --location --request POST 'https://heco.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_sendRawTransaction",
"params": ["0xd46e8dd67c5d32be8d46e8dd67c5d32be8058bb8eb970870f072445675058bb8eb970870f072445675"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "rlp: element is larger than containing list"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```


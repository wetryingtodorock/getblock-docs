---
title: one:hmyv2_getBalance \[POST\]
description: Returns the account balance of the specified address.
---

### Parameters


`DATA` - hex string

20-byte account address from which to retrieve the balance.

### Request

``` java
curl --location --request POST 'https://one.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "hmyv2_getBalance",
"params": ["0x227f6757289a86c13eee2e91c2e6eb03f2ed11a6"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": 0
}
```


---
title: gno:eth_getBalance \[POST\]
description: Returns the account balance of the specified address.
---

### Parameters


`DATA` - hex string

20-byte account address from which to retrieve the balance.

`QUANTITY|TAG` - hex string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://gno.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0xfe3b557e8fb62b89f4916b721be55ceb828dbd73", "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x3e20"
}
```


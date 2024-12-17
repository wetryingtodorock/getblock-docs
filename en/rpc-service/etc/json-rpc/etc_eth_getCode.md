---
title: etc:eth_getCode \[POST\]
description: Returns the code of the smart contract at the specified address. Besustores compiled smart contract code as a hexadecimal value.
---

### Parameters


`DATA` - integer or string

20-byte contract address.

`QUANTITY|TAG` - string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getCode",
"params": ["0x7eb4c9d6b763324eea4852f5d40985bbf0f29832", "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x"
}
```


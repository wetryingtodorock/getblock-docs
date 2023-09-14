---
title: etc:eth_call \[POST\]
description: Invokes a contract function locally and does not change the state of theblockchain.You can interact with contracts using eth_sendRawTransaction oreth_call.If revert reason is enabled with --revert-reason-enabled, the eth_callerror response will include the revert reason.
---

### Parameters


`OBJECT` - json object

Transaction call object.

`QUANTITY|TAG` - string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_call",
"params": [{"to": "0x69498dd54bd25aa0c886cf1f8b8ae0856d55ff13", "value": "0x1"}, "latest"],
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


---
title: eth:admin_logsRemoveCache  {disallowed} - Ethereum
description: Example code for the eth:admin_logsRemoveCache  {disallowed} ws method. Сomplete guide on how to use eth:admin_logsRemoveCache  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`fromBlock` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

`toBlock` - None

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin_logsRemoveCache",
"params": [null, null],
"id": "getblock.io"}
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


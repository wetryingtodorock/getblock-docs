---
title: eth:ibft_getValidatorsByBlockNumber  {disallowed} - Ethereum
description: Example code for the eth:ibft_getValidatorsByBlockNumber  {disallowed} ws method. Сomplete guide on how to use eth:ibft_getValidatorsByBlockNumber  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "ibft_getValidatorsByBlockNumber",
"params": [null],
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


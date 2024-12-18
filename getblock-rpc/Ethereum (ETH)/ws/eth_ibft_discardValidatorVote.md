---
title: ibft_discardValidatorVote  {disallowed} - Ethereum
description: Example code for the ibft_discardValidatorVote  {disallowed} ws method. Сomplete guide on how to use ibft_discardValidatorVote  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

20-byte address of proposed validator.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "ibft_discardValidatorVote",
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


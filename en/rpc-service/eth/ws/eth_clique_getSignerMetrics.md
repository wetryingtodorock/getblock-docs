---
title: eth:clique_getSignerMetrics  {disallowed} - Ethereum
description: Example code for the eth:clique_getSignerMetrics  {disallowed} ws method. Сomplete guide on how to use eth:clique_getSignerMetrics  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`fromBlockNumber` - None

Integer representing a block number or the string tag earliest, as
described in Block Parameter.

`toBlockNumber` - None

Integer representing a block number or one of the string tags latest or
pending, as described in Block Parameter

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "clique_getSignerMetrics",
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


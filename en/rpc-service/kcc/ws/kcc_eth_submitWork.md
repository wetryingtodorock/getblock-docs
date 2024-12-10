---
title: kcc:eth_submitWork  {disallowed} - KuCoin Community Chain
description: Example code for the kcc:eth_submitWork  {disallowed} ws method. Сomplete guide on how to use kcc:eth_submitWork  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - string

The nonce found (64 bits)

`data` - string

The header’s pow-hash (256 bits)

`data` - string

The mix digest (256 bits)

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_submitWork",
"params": [null, null, null],
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


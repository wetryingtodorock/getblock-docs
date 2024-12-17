---
title: eea_sendRawTransaction  {disallowed} - Ethereum
description: Example code for the eea_sendRawTransaction  {disallowed} ws method. Сomplete guide on how to use eea_sendRawTransaction  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

Signed RLP-encoded private transaction.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eea_sendRawTransaction",
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


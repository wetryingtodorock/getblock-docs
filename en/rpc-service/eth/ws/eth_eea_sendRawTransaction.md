---
title: eth:eea_sendRawTransaction \[WebSocket\] {disallowed}
description: Distributes the private transaction, generates the privacy markertransaction and submits it to the transaction pool, and returns thetransaction hash of the privacy marker transaction.The signed transaction passed as an input parameter includes theprivateFrom, privateFor or privacyGroupId, and restriction fields.The gas and gasPrice are used by the privacy marker transaction not theprivate transaction itself.To avoid exposing your private key, create signed transactions offlineand send the signed transaction data using eea_sendRawTransaction.
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


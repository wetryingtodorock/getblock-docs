---
title: avax:avax.export \[POST\] {disallowed}
description: Export an asset from the C-Chain to the X-Chain. After calling thismethod, you must call avm.import on the X-Chain to complete thetransfer.
---

### Parameters


`to` - string

the X-Chain address the asset is sent to.

`amount` - int

amount of the asset to send.

`assetID` - string

ID of the asset. To export AVAX use "AVAX" as the assetID.

`baseFee` - int

base fee that should be used when creating the transaction. If ommitted,
a suggested fee will be used.

`username` - string

user that controls the address that transaction will be sent from.

`password` - string

user's password

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "avax.export",
"params": [null, null, null, null, null, null],
"id": "getblock.io"}'
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


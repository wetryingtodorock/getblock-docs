---
title: trx:buildTransaction(TransferAssetContract) \[POST\] {disallowed}
description: Create a transaction, different transaction types have differentparametersthis is an example of TransferAssetContract
---

### Parameters


`from` - data, 20 bytes

The address the transaction is sent from.

`to` - data, 20 bytes

The address the transaction is directed to.

`tokenId` - QUANTITY

token ID

`tokenValue` - QUANTITY

The transfer amount of TRC10

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/mainnet/fullnode/jsonrpc' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "buildTransaction",
"params": ["0xC4DB2C9DFBCB6AA344793F1DDA7BD656598A06D8", "0x95FD23D3D2221CFEF64167938DE5E62074719E54", "1000016", 20],
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


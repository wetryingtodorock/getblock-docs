---
title: btc:utxoupdatepsbt \[POST\]
description: Updates all segwit inputs and outputs in a PSBT with data from outputdescriptors, the UTXO set or the mempool.
---

### Parameters


`psbt` - string, required

A base64 string of a PSBT

`descriptors` - json array, optional

An array of either strings or objects

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "utxoupdatepsbt",
"params": ["psbt", null],
"id": "getblock.io"}'
```


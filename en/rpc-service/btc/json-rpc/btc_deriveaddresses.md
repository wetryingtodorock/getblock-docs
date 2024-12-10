---
title: btc:deriveaddresses - Bitcoin
description: Example code for the btc:deriveaddresses json-rpc method. Сomplete guide on how to use btc:deriveaddresses json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`descriptor` - string, required

The descriptor.

`range` - numeric or array, optional

If a ranged descriptor is used, this specifies the end or the range (in
\[begin,end\] notation) to derive.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "sendrawtransaction",
"params": ["descriptor", null],
"id": "getblock.io"}'
```


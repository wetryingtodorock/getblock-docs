---
title: btc:decoderawtransaction \[POST\]
description: Return a JSON object representing the serialized, hex-encodedtransaction.
---

### Parameters


`hexstring` - string, required

The transaction hex string

`iswitness` - boolean, optional, default=depends on heuristic tests

Whether the transaction hex is a serialized witness transaction.

If iswitness is not present, heuristic tests will be used in decoding.

If true, only witness deserialization will be tried.

If false, only non-witness deserialization will be tried.

This boolean should reflect whether the transaction has inputs (e.g.
fully valid, or on-chain transactions), if known by the caller.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "decoderawtransaction",
"params": ["hexstring", null],
"id": "getblock.io"}'
```

###  Response

``` java
null
```


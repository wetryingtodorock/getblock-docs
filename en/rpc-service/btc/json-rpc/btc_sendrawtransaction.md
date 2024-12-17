---
title: btc:sendrawtransaction \[POST\]
description: Submit a raw transaction (serialized, hex-encoded) to local node andnetwork.Note that the transaction will be sent unconditionally to all peers, sousing this for manual rebroadcast may degrade privacy by leaking thetransactions origin, as nodes will normally not rebroadcast non-wallettransactions already in their mempool.
---

### Parameters


`hexstring` - string, required

The hex string of the raw transaction

`maxfeerate` - numeric or string, optional, default=0.10

Reject transactions whose fee rate is higher than the specified value,
expressed in BTC/kB.

Set to 0 to accept any fee rate.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "sendrawtransaction",
"params": ["hexstring", null],
"id": "getblock.io"}'
```

###  Response

``` java
null
```


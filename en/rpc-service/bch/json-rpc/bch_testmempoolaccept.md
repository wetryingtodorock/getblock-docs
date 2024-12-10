---
title: bch:testmempoolaccept - Bitcoin Cash
description: Example code for the bch:testmempoolaccept json-rpc method. Сomplete guide on how to use bch:testmempoolaccept json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`rawtxs` - json array, required

An array of hex strings of raw transactions. Length must be one for now.

`maxfeerate` - numeric or string, optional, default=0.10

Reject transactions whose fee rate is higher than the specified value,
expressed in BTC/kB

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "testmempoolaccept",
"params": [["rawtxs"], null],
"id": "getblock.io"}'
```

###  Response

``` java
null
```


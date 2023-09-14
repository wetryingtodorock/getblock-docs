---
title: btc:createrawtransaction \[POST\]
description: Create a transaction spending the given inputs and creating new outputs.Outputs can be addresses or data.Returns hex-encoded raw transaction.Note that the transaction’s inputs are not signed, and it is not storedin the wallet or transmitted to the network.
---

### Parameters


`inputs` - json array, required

A json array of json objects

`outputs` - json array, required

The outputs (key-value pairs), where none of the keys are duplicated.

`locktime` - numeric, optional, default=0

Raw locktime. Non-0 value also locktime-activates inputs

`replaceable` - boolean, optional, default=false

Marks this transaction as BIP125 replaceable.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "createrawtransaction",
"params": [[{"txid": "myid", "vout": 0}], [{"data": "00010203"}], null, null],
"id": "getblock.io"}'
```

###  Response

``` java
null
```


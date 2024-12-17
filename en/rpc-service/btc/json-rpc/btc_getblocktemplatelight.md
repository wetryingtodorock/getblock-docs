---
title: btc:getblocktemplatelight \[POST\] {disallowed}
description: If the request parameters include a mode key, that is used toexplicitly select between the default template request or aproposal.It returns data needed to construct a block to work on.For full specification, see the getblocktemplatelight spec in the docfolder, and BIP22/BIP23.
---

### Parameters


`template_request` - json object, optional

A json object in the following spec

`additional_txs` - json array, optional, default=\[\]

Hex encoded transactions to add to the block (each tx must be unique and
valid)

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getblocktemplatelight",
"params": [null, null],
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


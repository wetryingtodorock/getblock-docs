---
title: doge:createrawtransaction \[POST\]
description: Creates a raw transaction spending given inputs (a list of dictionaries,each containing a transaction id and an output number), sending to givenaddress(es).
---

### Parameters


`inputs` - list of dict

A list of {“txid”: txid, “vout”: n} dictionaries.

`outputs` - dict

A dictionary mapping (public) addresses to the amount they are to be
paid.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "createrawtransaction",
"params": [[{"txid": "txidone", "vout": 100}, {"txid": "txidtwo", "vout": 10}], {"addressone": 10, "addresstwo": 100}],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": null
}
```


---
title: bch:logging \[POST\] {disallowed}
description: Gets and sets the logging configuration.When called without an argument, returns the list of categories withstatus that are currently being debug logged or not.When called with arguments, adds or removes categories from debuglogging and return the lists above.The arguments are evaluated in order “include”, “exclude”.If an item is both included and excluded, it will thus end up beingexcluded.The valid logging categories are net, tor, mempool, http, bench, zmq,walletdb, rpc, estimatefee, addrman, selectcoins, reindex, cmpctblock,rand, prune, proxy, mempoolrej, libevent, coindb, qt, leveldb,validationIn addition, the following are available as category names with specialmeanings\- all, 1  represent all logging categories.\- none, 0  even if other logging categories are specified, ignoreall of them.
---

### Parameters


`include` - json array, optional

A json array of categories to add debug logging

`exclude` - json array, optional

A json array of categories to remove debug logging

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "logging",
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


---
title: geth:eth_subscribe \[POST\]
description: Subscriptions are created with a regular RPC call with eth_subscribe asmethod and the subscription name as first parameter. If successful itreturns the subscription id.
---

### Parameters


`name` - string

subscription name

`arguments` - array of string

optional arguments

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_subscribe",
"params": ["syncing", null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xe2ffeb2703bcf602d42922385829ce96"
}
```


---
title: geth:eth_unsubscribe \[POST\]
description: Subscriptions are cancelled with a regular RPC call with eth_unsubscribeas method and the subscription id as first parameter. It returns a boolindicating if the subscription was cancelled successful.
---

### Parameters


`id` - string

subscription id

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_unsubscribe",
"params": ["0xe2ffeb2703bcf602d42922385829ce96"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": true
}
```


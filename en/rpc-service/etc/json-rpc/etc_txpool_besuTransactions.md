---
title: etc:txpool_besuTransactions \[POST\]
description: Lists transactions in the node transaction pool.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "txpool_besuTransactions",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        {
            "hash": "0x8a66830098be4006a3f63a03b6e9b67aa721e04bd6b46d420b8f1937689fb4f1",
            "isReceivedFromLocalSource": true,
            "addedToPoolAt": "2019-03-21T01:35:50.911Z"
        },
        {
            "hash": "0x41ee803c3987ceb5bcea0fad7a76a8106a2a6dd654409007d9931032ea54579b",
            "isReceivedFromLocalSource": true,
            "addedToPoolAt": "2019-03-21T01:36:00.374Z"
        }
    ]
}
```


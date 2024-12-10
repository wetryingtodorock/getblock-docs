---
title: btg:getmempoolentry - Bitcoin Gold
description: Example code for the btg:getmempoolentry json-rpc method. Сomplete guide on how to use btg:getmempoolentry json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`txid` - string, required

The transaction id (musFot be in mempool)

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getmempoolentry",
"params": ["5c970c064d317658a8777ee56f192fe17d5b3afbe242d820b205c2291210f269"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "fees": {
            "base": 0.001,
            "modified": 0.001,
            "ancestor": 0.001,
            "descendant": 0.001
        },
        "vsize": 225,
        "weight": 900,
        "fee": 0.001,
        "modifiedfee": 0.001,
        "time": 1617958131,
        "height": 678425,
        "descendantcount": 1,
        "descendantsize": 225,
        "descendantfees": 100000,
        "ancestorcount": 1,
        "ancestorsize": 225,
        "ancestorfees": 100000,
        "wtxid": "d56bc87e605bef45e1e63f43ece2a08edc80c65c709c7be33df6fa3c7f34688b",
        "depends": [],
        "spentby": [],
        "bip125-replaceable": false,
        "unbroadcast": false
    }
}
```


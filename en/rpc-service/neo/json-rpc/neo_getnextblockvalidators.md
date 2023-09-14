---
title: neo:getnextblockvalidators \[POST\]
description: Gets the validators list of the next block.result returns an array containing multiple validators.Every validator contains information about the public key, the votes,and whether it is a validator or not.The default vote of validator is 0 when voting has not started.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getnextblockvalidators",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": [
        {
            "publickey": "03aa052fbcb8e5b33a4eefd662536f8684641f04109f1d5e69cdda6f084890286a",
            "votes": "0",
            "active": true
        }
    ],
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```


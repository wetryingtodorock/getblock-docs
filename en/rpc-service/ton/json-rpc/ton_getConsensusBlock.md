---
title: ton:/getConsensusBlock \[GET\]
description: Get consensus block and its update timestamp.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://ton.getblock.io/mainnet/getConsensusBlock' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "ok": true,
    "result": {
        "consensus_block": 30517698,
        "timestamp": 1687338534.241151
    }
}
```


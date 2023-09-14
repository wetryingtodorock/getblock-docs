---
title: geth:txpool_inspect \[POST\]
description: The inspect inspection property can be queried to list a textual summaryof all the transactions currently pending for inclusion in the nextblock(s), as well as the ones that are being scheduled for futureexecution only. This is a method specifically tailored to developers toquickly see the transactions in the pool and find any potential issues.The result is an object with two fields pending and queued. Each ofthese fields are associative arrays, in which each entry maps anorigin-address to a batch of scheduled transactions. These batchesthemselves are maps associating nonces with transactions summarystrings.Please note, there may be multiple transactions associated with the sameaccount and nonce. This can happen if the user broadcast mutliple oneswith varying gas allowances (or even completely different transactions).
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "txpool_inspect",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "pending": {
            "0x000251Bd7762a21Df45175E6E571e83f68d15f3E": {
                "1": "0x63A0e8E7C9e86cF58E188b98F55CedEE42c3C902: 455000000000000 wei + 21000 gas \u00d7 7000000000 wei"
            },
            "0x0003BE8bd8dBa04Ac4dE888A9ea02AcF73b61700": {
                "1": "0xcf2F6FB91AE5D2a7c7d736c8F89ae51a8A3f57d2: 455000000000000 wei + 21000 gas \u00d7 7000000000 wei"
            },
            "0x000DB5cb74A30bbc2F21A3F3DD501E8E0585816a": {
                "1": "0x97A363e191f1F01459b2a9987eDd7C01C962f4CE: 455000000000000 wei + 21000 gas \u00d7 7000000000 wei"
            }
        }
    }
}
```


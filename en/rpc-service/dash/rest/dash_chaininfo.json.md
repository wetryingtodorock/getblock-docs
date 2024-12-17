---
title: /chaininfo.json - Dash
description: Example code for the /chaininfo.json rest method. Сomplete guide on how to use /chaininfo.json rest in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://dash.getblock.io/mainnet//chaininfo.json' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "bestblockhash": "000000000000001d507d43a6567386e443deecbe1922f2e4b11bcd0ccb401ada",
    "bip9_softforks": {
        "bip147": {
            "since": 939456,
            "start_time": 1524477600,
            "status": "active",
            "timeout": 1556013600
        },
        "csv": {
            "since": 622944,
            "start_time": 1486252800,
            "status": "active",
            "timeout": 1517788800
        }
    },
    "blocks": 1891101,
    "chain": "main",
    "chainwork": "0000000000000000000000000000000000000000000086af3b0dda499d4811c2",
    "difficulty": 115067188.1449891,
    "headers": 1891101,
    "initialblockdownload": false,
    "mediantime": 1687338859,
    "pruned": false,
    "size_on_disk": 34394938419,
    "softforks": [
        {
            "id": "bip34",
            "reject": {
                "status": true
            },
            "version": 2
        },
        {
            "id": "bip66",
            "reject": {
                "status": true
            },
            "version": 3
        },
        {
            "id": "bip65",
            "reject": {
                "status": true
            },
            "version": 4
        }
    ],
    "verificationprogress": 0.9999996194380817,
    "warnings": "Warning: unknown new rules activated (versionbit 8)"
}
```


---
title: trx:/wallet/getchainparameters - TRON
description: Example code for the trx:/wallet/getchainparameters rest method. Сomplete guide on how to use trx:/wallet/getchainparameters rest in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://trx.getblock.io/wallet/getchainparameters' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "chainParameter": [
        {
            "key": "getMaintenanceTimeInterval",
            "value": 21600000
        },
        {
            "key": "getAccountUpgradeCost",
            "value": 9999000000
        },
        {
            "key": "getCreateAccountFee",
            "value": 100000
        }
    ]
}
```


---
title: sol:getBlockProduction \[POST\]
description: Returns recent block production information from the current or previousepoch.
---

### Parameters


`Config` - object

Optional.

Configuration object containing the following optional fields: -
Commitment (optional) - range: object - Slot range to return block
production for. If parameter not provided, defaults to current epoch. -
firstSlot: u64 - first slot to return block production information for
(inclusive) - lastSlot: u64 (optional) - last slot to return block
production information for (inclusive). If parameter not provided,
defaults to the highest slot - identity: string (optional) - Only return
results for this validator identity (base-58 encoded)

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getBlockProduction",
"params": [null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "context": {
            "slot": 123033977
        },
        "value": {
            "byIdentity": {
                "12CUDzb3oe8RBQ4tYGqsuPsCbsVE4KWfktXRihXf8Ggq": [
                    84,
                    77
                ],
                "12ashmTiFStQ8RGUpi1BTCinJakVyDKWjRL6SWhnbxbT": [
                    176,
                    163
                ],
                "12oRmi8YDbqpkn326MdjwFeZ1bh3t7zVw8Nra2QK2SnR": [
                    84,
                    83
                ],
                "13442mSWLHjWwz3A39qjDEZzZR1jUWKNzgphNBsrS7xy": [
                    52,
                    51
                ],
                "138KHwTqKNWGLoo8fK5i8UxYtwoC5tC8o7M9rY1CDEjT": [
                    84,
                    81
                ],
                "13ftbVP7cpBp3JrQoXjfSWbNX8uS9ABLus4oZ4KaGodL": [
                    92,
                    91
                ]
            },
            "range": {
                "firstSlot": 122688000,
                "lastSlot": 123033977
            }
        }
    }
}
```


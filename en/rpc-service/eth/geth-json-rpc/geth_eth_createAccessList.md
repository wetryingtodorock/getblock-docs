---
title: geth:eth_createAccessList \[POST\]
description: This method creates an EIP2930 type accessList based on a givenTransaction. The accessList contains all storage slots and addressesread and written by the transaction, except for the sender account andthe precompiles. This method uses the same transaction call object andblockNumberOrTag object as eth_call. An accessList can be used tounstuck contracts that became inaccessible due to gas cost increases.
---

### Parameters


`transaction` - object

TransactionCall object

`blockNumberOrTag` - object

Optional, blocknumber or latest or pending

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_createAccessList",
"params": [{"from": "0x8cd02c6cbd8375b39b06577f8d50c51d86e8d5cd", "data": "0x608060806080608155"}, "pending"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "accessList": [
            {
                "address": "0xa02457e5dfd32bda5fc7e1f1b008aa5979568150",
                "storageKeys": [
                    "0x0000000000000000000000000000000000000000000000000000000000000081"
                ]
            }
        ],
        "gasUsed": "0x125f8"
    }
}
```


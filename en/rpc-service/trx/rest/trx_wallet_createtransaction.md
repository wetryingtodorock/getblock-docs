---
title: trx:/wallet/createtransaction \[POST\]
description: Create a TRX transfer transaction. If to_address does not exist, thencreate the account on the blockchain.
---

### Parameters


`to_address` - string

To_address is the transfer address, converted to a hex string

`owner_address` - string

Owner_address is the transfer address, converted to a hex string

`amount` - int64

Amount is the transfer amount,the unit is sun

`permission_id` - int32

Optional, for multi-signature use

`visible` - boolean

Optional.Whehter the address is in base58 format.

`extra_data` - string

Optional, totes on the transaction, HEX format

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/createtransaction' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"to_address": "414a5fe0179f2dd9c900194e63d661863cd0ade7b0", "owner_address": "41718de6b323652d1257437ace160c4f4198aae4e1", "amount": 1000}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "message": {  
      "txID":"9908eed564650eed0027b84b18adb934e401e39a62d7c8964224fc723914f551",
      "raw_data":{  
          "contract":[  
            {  
                "parameter":{  
                  "value":{  
                      "amount":1000,
                      "owner_address":"41718de6b323652d1257437ace160c4f4198aae4e1",
                      "to_address":"414a5fe0179f2dd9c900194e63d661863cd0ade7b0"
                  },
                  "type_url":"type.googleapis.com/protocol.TransferContract"
                },
                "type":"TransferContract"
            }
          ],
          "ref_block_bytes":"00b0",
          "ref_block_hash":"3f1bc96dc80e7f61",
          "expiration":1548974130000,
          "timestamp":1548974072663
          }
      }
}
```


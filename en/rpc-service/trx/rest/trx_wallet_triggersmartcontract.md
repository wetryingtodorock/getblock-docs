---
title: /wallet/triggersmartcontract  {disallowed} - TRON
description: Example code for the /wallet/triggersmartcontract  {disallowed} rest method. Сomplete guide on how to use /wallet/triggersmartcontract  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Address that triggers the contract, converted to a hex string.

`contract_address` - string

Contract address, converted to a hex string

`function_selector` - string

Function call, must not be left blank

`parameter` - string

Parameter encoding needs to be in accordance with the ABI rules, the
rules are more complicated, users can use the ethers library to
encode,For details, please refer to the document-Guide-Smart
Contract-Best Practice-Parameter Encoding and Decoding.

`fee_limit` - int32

Maximum TRX consumption, measured in SUN (1 TRX = 1,000,000 SUN).

`call_value` - int32

Amount of TRX transferred with this transaction, measured in SUN (1 TRX
= 1,000,000 SUN).

`permission_id` - int32

Optional, for multi-signature

`visible` - boolean

Optional. Whehter the address is in base58check format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/triggersmartcontract' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```


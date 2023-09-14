---
title: trx:/wallet/triggerconstantcontract \[POST\] {disallowed}
description: Invoke the readonly function (modified by the view or pure modifier) ofa contract for contract data query or Invoke the non-readonly functionof a contract for predicting whether the transaction can be successfullyexecuted or estimating the energy consumptionTriggerConstantContract operation will not generate an on-chaintransaction, nor will it change the status of the current node.For estimating energy use triggerconstantcontract to call thenon-readonly method of the contract, and the energy_used field in thereturned value is the energy consumption. Therefore, the fee_limit ofthe transaction can be set to energy_used x energy unit price.
---

### Parameters


`owner_address` - string

Owner address that triggers the contract. If visible=true, use
base58check format, otherwise use hex format. For constant call you can
use the all-zero address.

`contract_address` - string

Smart contract address. If visible=true, use base58check format,
otherwise use hex format.

`function_selector` - string

Function call, must not be left blank.

`parameter` - string

Parameter encoding needs to be in accordance with the ABI rules, the
rules are more complicated, users can use the ethers library to
encode,For details, please refer to the document-Guide-Smart
Contract-Best Practice-Parameter Encoding and Decoding.

`visible` - string

Optional.Whehter the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/triggerconstantcontract' \
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


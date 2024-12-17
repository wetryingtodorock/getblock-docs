---
title: trx:/wallet/triggerconstantcontract  {disallowed} - TRON
description: Example code for the trx:/wallet/triggerconstantcontract  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/triggerconstantcontract  {disallowed} rest in GetBlock.io Web3 documentation.
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


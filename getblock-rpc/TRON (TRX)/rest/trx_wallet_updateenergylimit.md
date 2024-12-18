---
title: /wallet/updateenergylimit  {disallowed} - TRON
description: Example code for the /wallet/updateenergylimit  {disallowed} rest method. Сomplete guide on how to use /wallet/updateenergylimit  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Transaction creator address, in hex string format.

`contract_address` - string

The address of the contract to be modified, in hex string format.

`origin_energy_limit` - int32

The maximum energy the creator sets. The greatest amount of energy the
creator consumes during contract execution or creation process.

`permission_id` - int32

Optional. Whehter the address is in base58 format.

`visible` - boolean

Optional. Whehter the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/updateenergylimit' \
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


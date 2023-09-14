---
title: trx:/wallet/updateenergylimit \[POST\] {disallowed}
description: Update the origin_energy_limit parameter of a smart contractStarting with Java-Tron Odyssey 3.2 release, this parameter is requiredfor deploying new contracts, and the value should be larger than 0. Forcontracts already deployed on the Mainnet prior to Odyssey 3.2, thevalue is stored as 0, but treated as maximum = 10,000,000.
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


---
title: xem:/account/get/forwarded \[GET\]
description: Given a delegate (formerly known as remote) accounts address, gets theAccountMetaDataPair for the account for which the given account is thedelegate account. If the given account address is not a delegate accountfor any account, the request returns the AccountMetaDataPair for thegiven address.
---

### Parameters


`address` -

The address of the delegate account.

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/account/get/forwarded?address=NC4T246ALCPNBTAOCSC5EAVFMDFBOACSQAF6WKHV'
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "account": {
        "address": "NC4T246ALCPNBTAOCSC5EAVFMDFBOACSQAF6WKHV",
        "balance": 0,
        "harvestedBlocks": 0,
        "importance": 0.0,
        "label": null,
        "multisigInfo": {},
        "publicKey": null,
        "vestedBalance": 0
    },
    "meta": {
        "cosignatories": [],
        "cosignatoryOf": [],
        "remoteStatus": "INACTIVE",
        "status": "LOCKED"
    }
}
```


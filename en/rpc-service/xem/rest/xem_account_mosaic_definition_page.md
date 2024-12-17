---
title: xem:/account/mosaic/definition/page \[GET\]
description: Gets an array of mosaic definition objects for a given account address.The parent parameter is optional. If supplied, only mosaic definitionsfor the given parent namespace are returned. The id parameter isoptional and allows retrieving mosaic definitions in batches of 25mosaic definitions.
---

### Parameters


`address` -

The address of the account.

`parent` -

The optional parent namespace id.

`id` -

The optional mosaic definition database id up to which mosaic
definitions are returned.

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/account/mosaic/definition/page?address=NC4T246ALCPNBTAOCSC5EAVFMDFBOACSQAF6WKHV'
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "data": [
        {
            "creator": "10cfe522fe23c015b8ab24ef6a0c32c5de78eb55b2152ed07b6a092121187100",
            "id": {
                "namespaceId": "makoto.metal.coins",
                "name": "silver coin"
            },
            "description": "Real silver coins, pure silver",
            "properties": [
                {
                    "name": "divisibility",
                    "value": "0"
                },
                {
                    "name": "initialSupply",
                    "value": "1000"
                },
                {
                    "name": "supplyMutable",
                    "value": "false"
                },
                {
                    "name": "transferable",
                    "value": "true"
                }
            ]
        }
    ]
}
```


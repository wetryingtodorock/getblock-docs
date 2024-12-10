---
title: xem:/account/namespace/page - NEM
description: Example code for the xem:/account/namespace/page rest method. Сomplete guide on how to use xem:/account/namespace/page rest in GetBlock.io Web3 documentation.
---

### Parameters


`address` -

The address of the account.

`parent` -

The optional parent namespace id.

`id` -

The optional namespace database id up to which namespaces are returned.

`pageSize` -

The (optional) number of namespaces to be returned.

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/account/namespace/page?address=NC4T246ALCPNBTAOCSC5EAVFMDFBOACSQAF6WKHV&pageSize=5'
 --header 'x-api-key:YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "data": [
        {
            "fqn": "makoto.metal.coins",
            "owner": "TD3RXTHBLK6J3UD2BH2PXSOFLPWZOTR34WCG4HXH",
            "height": 13465
        }
    ]
}
```


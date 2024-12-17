---
title: theta:thetacli.NewKey \[POST\] {disallowed}
description: This API creates a new account (i.e. a private key/addres pair), andencrypts the private key under ~/.thetacli/keys/encrypted/ by default.
---

### Parameters


`password` - string

\-

T

h

e

p

a

s

s

w

o

r

d

f

o

r

t

h

e

n

e

w

a

c

c

o

u

n

t

.

### Request

``` java
curl --location --request POST 'https://theta.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "thetacli.NewKey",
"params": {},
"id": "getblock.io"}'
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


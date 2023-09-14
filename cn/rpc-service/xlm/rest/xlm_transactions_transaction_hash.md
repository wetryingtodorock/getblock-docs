---
title: xlm:/transactions/{transaction_hash} \[GET\]
description: The single transaction endpoint provides information on a specifictransaction.
---

### Parameters


`transaction_hash` - path

string, required

Transactions are commands that modify the ledger state and consist of
one or more operations.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet//transactions/339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_links": {
        "account": {
            "href": "https://xlm.getblock.io/accounts/GDY7XUWBA3N7SNGSQSNVQ5DUCIIB5PNNGV3OKE472CU4VW6ZTYN2UK66"
        },
        "effects": {
            "href": "https://xlm.getblock.io/transactions/339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601/effects{?cursor,limit,order}",
            "templated": true
        },
        "ledger": {
            "href": "https://xlm.getblock.io/ledgers/45678720"
        },
        "operations": {
            "href": "https://xlm.getblock.io/transactions/339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601/operations{?cursor,limit,order}",
            "templated": true
        },
        "precedes": {
            "href": "https://xlm.getblock.io/transactions?order=asc&cursor=196188608523145216"
        },
        "self": {
            "href": "https://xlm.getblock.io/transactions/339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601"
        },
        "succeeds": {
            "href": "https://xlm.getblock.io/transactions?order=desc&cursor=196188608523145216"
        },
        "transaction": {
            "href": "https://xlm.getblock.io/transactions/339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601"
        }
    },
    "created_at": "2023-04-04T10:14:50Z",
    "envelope_xdr": "AAAAAgAAAADx+9LBBtv5NNKEm1h0dBIQHr2tNXblE5/Qqcrb2Z4bqgAD0JUCbpu7AADYOAAAAAEAAAAAAAAAAAAAAABkK/i3AAAAAAAAAAEAAAABAAAAAETBzvdU5vmigYboQdYo6q6s50kcfy1YK9CQimEde+ncAAAAAwAAAAFPTkVIAAAAAGOKM5UEd5rHtExI4l+tgmNB/EkfSK+a1S4RwoR8S/KeAAAAAAAAAAGTcLxnBTvpiR3vfJAAAAAASFtiJAAAAAAAAAACHXvp3AAAAEC3Nj3qhxBX1k6FOx1aztDygvWjpYUnVQ3eyzgmxEN/DoJOpTYPQS4kRu9gCHdh/P0uJcOZkijBAjYvEHTIyMYD2Z4bqgAAAEDKhEOG9MwC8PtTz7J5+TRMLInp2rbrBhVCNy0rHzc1C5RjFGuN+g8MdpWg8Nb4IYE4PxZlQjPFixwykQsJ/tMD",
    "fee_account": "GDY7XUWBA3N7SNGSQSNVQ5DUCIIB5PNNGV3OKE472CU4VW6ZTYN2UK66",
    "fee_charged": "10000",
    "fee_meta_xdr": "AAAAAgAAAAMCuP8VAAAAAAAAAADx+9LBBtv5NNKEm1h0dBIQHr2tNXblE5/Qqcrb2Z4bqgAAAAABxMitAm6buwAA2DcAAAAAAAAAAAAAAAAAAAAAAQAAAAAAAAAAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAIAAAAAAAAAAAAAAAAAAAADAAAAAAK4/xUAAAAAZCvwhQAAAAAAAAABArkAgAAAAAAAAAAA8fvSwQbb+TTShJtYdHQSEB69rTV25ROf0KnK29meG6oAAAAAAcShnQJum7sAANg3AAAAAAAAAAAAAAAAAAAAAAEAAAAAAAAAAAAAAQAAAAAAAAAAAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAwAAAAACuP8VAAAAAGQr8IUAAAAA",
    "hash": "339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601",
    "id": "339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601",
    "ledger": 45678720,
    "max_fee": "250005",
    "memo_type": "none",
    "operation_count": 1,
    "paging_token": "196188608523145216",
    "preconditions": {
        "timebounds": {
            "max_time": "1680603319",
            "min_time": "0"
        }
    },
    "result_meta_xdr": "AAAAAgAAAAIAAAADArkAgAAAAAAAAAAA8fvSwQbb+TTShJtYdHQSEB69rTV25ROf0KnK29meG6oAAAAAAcShnQJum7sAANg3AAAAAAAAAAAAAAAAAAAAAAEAAAAAAAAAAAAAAQAAAAAAAAAAAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAwAAAAACuP8VAAAAAGQr8IUAAAAAAAAAAQK5AIAAAAAAAAAAAPH70sEG2/k00oSbWHR0EhAeva01duUTn9CpytvZnhuqAAAAAAHEoZ0Cbpu7AADYOAAAAAAAAAAAAAAAAAAAAAABAAAAAAAAAAAAAAEAAAAAAAAAAAAAAAAAAAAAAAAAAgAAAAAAAAAAAAAAAAAAAAMAAAAAArkAgAAAAABkK/iaAAAAAAAAAAEAAAAGAAAAAwK5AGoAAAACAAAAAETBzvdU5vmigYboQdYo6q6s50kcfy1YK9CQimEde+ncAAAAAEhbYiQAAAABT05FSAAAAABjijOVBHeax7RMSOJfrYJjQfxJH0ivmtUuEcKEfEvyngAAAAAAAAABk3C8Zg2bO1lN0flmAAAAAAAAAAAAAAAAAAAAAQK5AIAAAAACAAAAAETBzvdU5vmigYboQdYo6q6s50kcfy1YK9CQimEde+ncAAAAAEhbYiQAAAABT05FSAAAAABjijOVBHeax7RMSOJfrYJjQfxJH0ivmtUuEcKEfEvyngAAAAAAAAABk3C8ZQU76Ykd73yQAAAAAAAAAAAAAAAAAAAAAwK5AHgAAAAAAAAAAETBzvdU5vmigYboQdYo6q6s50kcfy1YK9CQimEde+ncAAAAGPC3wYYCOMICAAAR6AAAAksAAAAAAAAAAAAAAAABAAAAAAAAAAAAAAEAAABbb1CuEAAAABM0lcRzAAAAAgAAAAAAAAAAAAAAAAAAAAMAAAAAArjxrAAAAABkK6OxAAAAAAAAAAECuQCAAAAAAAAAAABEwc73VOb5ooGG6EHWKOqurOdJHH8tWCvQkIphHXvp3AAAABjwt8GGAjjCAgAAEegAAAJLAAAAAAAAAAAAAAAAAQAAAAAAAAAAAAABAAAAW29QrYYAAAATNJXEcwAAAAIAAAAAAAAAAAAAAAAAAAADAAAAAAK48awAAAAAZCujsQAAAAAAAAADArkAagAAAAEAAAAARMHO91Tm+aKBhuhB1ijqrqznSRx/LVgr0JCKYR176dwAAAABT05FSAAAAABjijOVBHeax7RMSOJfrYJjQfxJH0ivmtUuEcKEfEvyngAAAAGTcLxnf/////////8AAAABAAAAAQAapUlSkQtBAAAAAZNwvGYAAAAAAAAAAAAAAAECuQCAAAAAAQAAAABEwc73VOb5ooGG6EHWKOqurOdJHH8tWCvQkIphHXvp3AAAAAFPTkVIAAAAAGOKM5UEd5rHtExI4l+tgmNB/EkfSK+a1S4RwoR8S/KeAAAAAZNwvGd//////////wAAAAEAAAABABqlSVKRC0EAAAABk3C8ZQAAAAAAAAAAAAAAAA==",
    "result_xdr": "AAAAAAAAJxAAAAAAAAAAAQAAAAAAAAADAAAAAAAAAAAAAAABAAAAAETBzvdU5vmigYboQdYo6q6s50kcfy1YK9CQimEde+ncAAAAAEhbYiQAAAABT05FSAAAAABjijOVBHeax7RMSOJfrYJjQfxJH0ivmtUuEcKEfEvyngAAAAAAAAABk3C8ZQU76Ykd73yQAAAAAAAAAAAAAAAA",
    "signatures": [
        "tzY96ocQV9ZOhTsdWs7Q8oL1o6WFJ1UN3ss4JsRDfw6CTqU2D0EuJEbvYAh3Yfz9LiXDmZIowQI2LxB0yMjGAw==",
        "yoRDhvTMAvD7U8+yefk0TCyJ6dq26wYVQjctKx83NQuUYxRrjfoPDHaVoPDW+CGBOD8WZUIzxYscMpELCf7TAw=="
    ],
    "source_account": "GDY7XUWBA3N7SNGSQSNVQ5DUCIIB5PNNGV3OKE472CU4VW6ZTYN2UK66",
    "source_account_sequence": "175248662975273016",
    "successful": true,
    "valid_after": "1970-01-01T00:00:00Z",
    "valid_before": "2023-04-04T10:15:19Z"
}
```


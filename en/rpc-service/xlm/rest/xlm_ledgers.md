---
title: xlm:/ledgers \[GET\]
description: This endpoint lists all ledgers and can be used in streaming mode.Streaming mode allows you to listen for new ledgers as they close. Ifcalled in streaming mode, Horizon will start at the earliest knownledger unless a cursor is set, in which case it will start from thatcursor. By setting the cursor value to now, you can stream ledgers sinceyour request time.
---

### Parameters


`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

string, optional

A designation of the order in which records should appear. Options
include asc (ascending) or desc (descending). If this argument isn’t
set, it defaults to asc.

`limit` - query

integer, optional

The maximum number of records returned. The limit can range from 1 to
200 - an upper limit that is hardcoded in Horizon for performance
reasons. If this argument isn’t designated, it defaults to 10.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/ledgers?cursor=196188608523149313&limit=1' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_embedded": {
        "records": [
            {
                "_links": {
                    "effects": {
                        "href": "https://xlm.getblock.io/ledgers/45678721/effects{?cursor,limit,order}",
                        "templated": true
                    },
                    "operations": {
                        "href": "https://xlm.getblock.io/ledgers/45678721/operations{?cursor,limit,order}",
                        "templated": true
                    },
                    "payments": {
                        "href": "https://xlm.getblock.io/ledgers/45678721/payments{?cursor,limit,order}",
                        "templated": true
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/ledgers/45678721"
                    },
                    "transactions": {
                        "href": "https://xlm.getblock.io/ledgers/45678721/transactions{?cursor,limit,order}",
                        "templated": true
                    }
                },
                "base_fee_in_stroops": 100,
                "base_reserve_in_stroops": 5000000,
                "closed_at": "2023-04-04T10:14:56Z",
                "failed_transaction_count": 17,
                "fee_pool": "3678306.1969888",
                "hash": "c0744e9a2ff25b4a4ea27877aa65e2c8f3ade6a1a91a18a44d203d88266bd911",
                "header_xdr": "AAAAEySuEovXrDnv/JNEmwTCYTLjdK0Dczn9sAS813qcHVMZMgxYhjJvaiDREDxvQBQ9hkxfG8y9SRHtDaGax84sFNUAAAAAZCv4oAAAAAAAAAABAAAAAPsLErXhs5nB/PBjevRUYxi38TMxR/LbCU2ivvBEXjyTAAAAQAnCVS6SqU11pQMUQONdOpWqhEyb9wvmC6XzG13I3LPYgpuS4wCnkLQbrzaQi9NV8K9lUP6uPtd/WtewG/rhpAarZQ8xEr+QxyMQJ4SyZy3kQntJOnCDCHiQ30H9jsZ/nbXIfrMJrhS8oj3+OAjLDAyjecDJq1zpaAxK+myauiToArkAgQ6iHrPseVthAAAhdDlXq+AAAAEWAAAAAEleJmUAAABkAExLQAAAA+j9yVrmmfgOUWALZvjFjwncEVV0mVNg63xddRnSSY4gx+IHudHihq1T5HDppRYgU3eRF+uk/d3/QHxUaXtQqp5qpZiAMxv0Zk35/ASHEnAUtpU914icfL2NdipzItGdNq/V7WS4ZAhYfPzgs3v/91SvAYsHKvgB71sirU+HrFEleQAAAAA=",
                "id": "c0744e9a2ff25b4a4ea27877aa65e2c8f3ade6a1a91a18a44d203d88266bd911",
                "max_tx_set_size": 1000,
                "operation_count": 971,
                "paging_token": "196188612818108416",
                "prev_hash": "24ae128bd7ac39effc93449b04c26132e374ad037339fdb004bcd77a9c1d5319",
                "protocol_version": 19,
                "sequence": 45678721,
                "successful_transaction_count": 151,
                "total_coins": "105443902087.3472865",
                "tx_set_operation_count": 1000
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/ledgers?cursor=196188629997977600&limit=5&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/ledgers?cursor=196188612818108416&limit=5&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/ledgers?cursor=196188608523149313&limit=5&order=asc"
        }
    }
}
```


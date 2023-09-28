# Get All cores
**Method** : `GET`  
**URL** : `https://api.spacexdata.com/v4/cores`  
**Auth required** : `False`  
**Modulo** : Launches  
**Version** : v4  
**Query** : `False`

****

## Success Responses

**Code** : `200 OK`
```json
[
    {
        "block": null,
        "reuse_count": 0,
        "rtls_attempts": 0,
        "rtls_landings": 0,
        "asds_attempts": 0,
        "asds_landings": 0,
        "last_update": "Engine failure at T+33 seconds resulted in loss of vehicle",
        "launches": [
            "5eb87cd9ffd86e000604b32a"
        ],
        "serial": "Merlin1A",
        "status": "lost",
        "id": "5e9e289df35918033d3b2623"
    },
    ...
]
```

# Get Last Update per core with patch of launch
**Method** : `POST`  
**URL** : `https://api.spacexdata.com/v4/cores`  
**Auth required** : `False`  
**Modulo** : Launches  
**Version** : v4  
**Query** : 
```json
{
    "query": {
    },
    "options": {
        "select": {
            "last_update": 1
        },
        "populate": [
            {
                "path": "launches",
                "select":{
                    "links.patch": 1
                }
            }
        ]
    }
}
```

****

## Success Responses

**Code** : `200 OK`
```json
{
    "docs": [
        {
            "last_update": "Engine failure at T+33 seconds resulted in loss of vehicle",
            "launches": [
                {
                    "links": {
                        "patch": {
                            "small": "https://images2.imgbox.com/94/f2/NN6Ph45r_o.png",
                            "large": "https://images2.imgbox.com/5b/02/QcxHUb5V_o.png"
                        }
                    },
                    "id": "5eb87cd9ffd86e000604b32a"
                }
            ],
            "id": "5e9e289df35918033d3b2623"
        },
        ...
    ],
    "totalDocs": 83,
    "offset": 0,
    "limit": 10,
    "totalPages": 9,
    "page": 1,
    "pagingCounter": 1,
    "hasPrevPage": false,
    "hasNextPage": true,
    "prevPage": null,
    "nextPage": 2
}
```


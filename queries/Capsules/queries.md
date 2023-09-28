# Get All Capsules
**Method** : `GET`  
**URL** : `https://api.spacexdata.com/v4/capsules`  
**Auth required** : `False`  
**Modulo** : Capsules
**Version** : v4  
**Query** : `False`

## Success Responses

**Code** : `200 OK`
```json
[
    {
        "reuse_count": 1,
        "water_landings": 1,
        "land_landings": 0,
        "last_update": "Reentered after three weeks in orbit",
        "launches": [
            "5eb87cdeffd86e000604b330"
        ],
        "serial": "C101",
        "status": "retired",
        "type": "Dragon 1.0",
        "id": "5e9e2c5bf35918ed873b2664"
    },
    ...
]
```

# Get All Capsules with the Launches Patch
**Method** : `POST`  
**URL** : `https://api.spacexdata.com/v4/capsules`  
**Auth required** : `False`  
**Modulo** : Capsules  
**Version** : v4  
**Query** : 
```json
{
    "query": {
    },
    "options": {
        "populate": [
            {
                "path": "launches",
                "select": {
                    "links.patch": 1
                }
            }
        ]
    }
}
```

***
## Success Responses

**Code** : `200 OK`
```json
{
    "docs": [
        {
            "reuse_count": 0,
            "water_landings": 1,
            "land_landings": 0,
            "last_update": "Hanging in atrium at SpaceX HQ in Hawthorne ",
            "launches": [
                {
                    "links": {
                        "patch": {
                            "small": "https://images2.imgbox.com/fa/dc/FOUDQ0Sn_o.png",
                            "large": "https://images2.imgbox.com/04/6e/kniggvWD_o.png"
                        }
                    },
                    "id": "5eb87cdeffd86e000604b330"
                }
            ],
            "serial": "C101",
            "status": "retired",
            "type": "Dragon 1.0",
            "id": "5e9e2c5bf35918ed873b2664"
        },
        ...
    ],
    "totalDocs": 25,
    "offset": 0,
    "limit": 10,
    "totalPages": 3,
    "page": 1,
    "pagingCounter": 1,
    "hasPrevPage": false,
    "hasNextPage": true,
    "prevPage": null,
    "nextPage": 2
}
```

# Get All Capsules with a reuse greater than zero
**Method** : `POST`  
**URL** : `https://api.spacexdata.com/v4/capsules`  
**Auth required** : `False`  
**Modulo** : Capsules  
**Version** : v4  
**Query** : 
```json
{
    "query": {
        "reuse_count": { "$gt": 0 }
    },
    "options": {
        "select": ["reuse_count", "last_update", "serial", "status"]
    }
}
```

***
## Success Responses

**Code** : `200 OK`
```json
{
    "docs": [
        {
            "reuse_count": 2,
            "last_update": "As of January 8, 2020: Arrived at Port of LA after splashdown following CRS-19 mission",
            "serial": "C106",
            "status": "active",
            "id": "5e9e2c5bf3591880643b2669"
        },
        ...
    ],
    "totalDocs": 10,
    "offset": 0,
    "limit": 10,
    "totalPages": 1,
    "page": 1,
    "pagingCounter": 1,
    "hasPrevPage": false,
    "hasNextPage": false,
    "prevPage": null,
    "nextPage": null
}
```

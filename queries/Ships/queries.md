# Get All Ships
**Method** : `GET`  
**URL** : `https://api.spacexdata.com/v4/ships`  
**Auth required** : `False`  
**Modulo** : Ships  
**Version** : v4  
**Query** : `False`

****
## Success Responses

**Code** : `200 OK`
```json
[
    {
        "last_ais_update": null,
        "legacy_id": "AMERICANCHAMPION",
        "model": null,
        "type": "Tug",
        "roles": [
            "Support Ship",
            "Barge Tug"
        ],
        "imo": 7434016,
        "mmsi": 367020820,
        "abs": 571252,
        "class": 7604342,
        "mass_kg": 266712,
        "mass_lbs": 588000,
        "year_built": 1976,
        "home_port": "Port of Los Angeles",
        "status": "",
        "speed_kn": null,
        "course_deg": null,
        "latitude": null,
        "longitude": null,
        "link": "https://www.marinetraffic.com/en/ais/details/ships/shipid:434663/mmsi:367020820/imo:7434016/vessel:AMERICAN_CHAMPION",
        "image": "https://i.imgur.com/woCxpkj.jpg",
        "name": "American Champion",
        "active": false,
        "launches": [
            "5eb87cdeffd86e000604b330",
            "5eb87cdfffd86e000604b331"
        ],
        "id": "5ea6ed2d080df4000697c901"
    },
]
```

# Get All Ships with only Img and name
**Method** : `POST`  
**URL** : `https://api.spacexdata.com/v4/ships`  
**Auth required** : `False`  
**Modulo** : Ships  
**Version** : v4  
**Query** : 
```json
{
    "query": {
    },
    "options": {
        "select": {
            "image": 1,
            "name": 1
        }
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
            "image": "https://i.imgur.com/woCxpkj.jpg",
            "name": "American Champion",
            "id": "5ea6ed2d080df4000697c901"
        },
        ...
    ],
    "totalDocs": 29,
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
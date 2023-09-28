# Get ID Crews by launch
**Method** : `POST`  
**URL** : `https://api.spacexdata.com/v4/launches`  
**Auth required** : `False`  
**Modulo** : Launches  
**Version** : v4  
**Query** :
****
```json
{
  "query": {
      "flight_number": <number>
  },
  "options": {
      "select": ["crew", "flight_number"],
      "pagination": false
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
            "crew": [],
            "flight_number": 100,
            "id": "5ed981d91f30554030d45c2a"
        }
    ],
    "totalDocs": 1,
    "offset": 0,
    "limit": 1,
    "totalPages": 1,
    "page": 1,
    "pagingCounter": 1,
    "hasPrevPage": false,
    "hasNextPage": false,
    "prevPage": null,
    "nextPage": null
}
```

---
# Get details launches by ID
**Method** : `POST`  
**URL** : `https://api.spacexdata.com/v4/launches`  
**Auth required** : `False`  
**Modulo** : Launches  
**Version** : v4  
**Query** :
****
```json
{
  "query": {
      "flight_number": <number>
  },
  "options": {
      "select": ["crew", "flight_number", "details"],
      "pagination": false
  }
}
```
****

## Success Responses
**Code** : `200 OK`
****
```json
{
    "docs": [
        {
            "details": "This mission will launch the tenth batch of operational Starlink satellites, which are expected to be version 1.0, from LC-39A, Kennedy Space Center. It is the eleventh Starlink launch overall. The satellites will be delivered to low Earth orbit and will spend a few weeks maneuvering to their operational altitude of 550 km. This mission is includes rideshare payloads, SkySats 19-21, on top of the Starlink stack. The booster for this mission is expected to land on an ASDS.",
            "crew": [],
            "flight_number": 100,
            "id": "5ed981d91f30554030d45c2a"
        }
    ],
    "totalDocs": 1,
    "offset": 0,
    "limit": 1,
    "totalPages": 1,
    "page": 1,
    "pagingCounter": 1,
    "hasPrevPage": false,
    "hasNextPage": false,
    "prevPage": null,
    "nextPage": null
}
```

---
# Get All launches with Patches
**Method** : `POST`  
**URL** : `https://api.spacexdata.com/v4/launches`  
**Auth required** : `False`  
**Modulo** : Launches  
**Version** : v4  
**Query** :
****
```json
{
  "query": {
      "flight_number": <number>
  },
  "options": {
      "select": ["links.patch"],
      "pagination": false
  }
}
```
****

## Success Responses
**Code** : `200 OK`
****
```json
{
  "docs": [
    {
      "links": {
        "patch": {
          "small": "https://images2.imgbox.com/ab/5a/Pequxd5d_o.png",
          "large": "https://images2.imgbox.com/92/e4/7Cf6MLY0_o.png"
        }
      },
      "id": "5eb87cdcffd86e000604b32e"
    }
  ],
  "totalDocs": 1,
  "offset": 0,
  "limit": 1,
  "totalPages": 1,
  "page": 1,
  "pagingCounter": 1,
  "hasPrevPage": false,
  "hasNextPage": false,
  "prevPage": null,
  "nextPage": null
}
```

***
# Get Others
**Method** : `POST`  
**URL** : `https://api.spacexdata.com/v4/launches`  
**Auth required** : `False`  
**Modulo** : Launches  
**Version** : v4  
**Query** :
****
```json
{
  "query": {
  },
  "options": {
      "select": {"links": 1, "_id": 0},
      "pagination": false
  }
}
```
****

## Success Responses
**Code** : `200 OK`
****
```json
{
  "docs": [
    {
      "links": {
        "patch": {
          "small": "https://images2.imgbox.com/94/f2/NN6Ph45r_o.png",
          "large": "https://images2.imgbox.com/5b/02/QcxHUb5V_o.png"
        },
        "reddit": {
          "campaign": null,
          "launch": null,
          "media": null,
          "recovery": null
        },
        "flickr": {
          "small": [],
          "original": []
        },
        "presskit": null,
        "webcast": "https://www.youtube.com/watch?v=0a_00nJ_Y88",
        "youtube_id": "0a_00nJ_Y88",
        "article": "https://www.space.com/2196-spacex-inaugural-falcon-1-rocket-lost-launch.html",
        "wikipedia": "https://en.wikipedia.org/wiki/DemoSat"
      }
    },
    ...
}
```

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
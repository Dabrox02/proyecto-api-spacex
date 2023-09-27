# SpaceX
## How to Make a Query

All routes add `/query`

- `https://api.spacexdata.com/v4/capsules/query`

The default body for /query routes is:

```js
{
  "query": {},
  "options": {}
}
```

### Query Object
Query object accepts any valid MongoDB find() query.
See more [here](https://www.mongodb.com/docs/manual/tutorial/query-documents/).

```js
{
  "query": {
    "status": "retired",
    "$text": {
      "$search": "Hanging"
    }
  },
  "options": {
  }
}
```

### Options Object
Accepts any of the options documented [here](https://github.com/aravindnc/mongoose-paginate-v2#modelpaginatequery-options-callback)

- `select` { Object | String } - Fields to return (by default returns all fields). Documentation
- `sort` { Object | String } - Sort order. Documentation
- `offset` { Number } - Use offset or page to set skip position
- `page` { Number }
- `limit` { Number }
- `pagination` { Boolean } - If set to false, it will return all docs without adding limit condition. (Default: True)
- `populate` {Array | Object | String} - Paths which should be populated with other documents.


### Default Return
```js
{
    "docs": [],
    "totalDocs": 0,
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
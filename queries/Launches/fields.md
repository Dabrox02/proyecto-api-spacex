# Campos Launches

**URL**: `https://api.spacexdata.com/v4/launches`

| Campo                        | Tipo       | Valores Permitidos                        | Valor Predeterminado | Requerido |
|------------------------------|------------|------------------------------------------|-----------------------|-----------|
| flight_number                | Number     |                                          |                       | Sí        |
| name                         | String     |                                          |                       | Sí        |
| date_utc                     | String     |                                          |                       | Sí        |
| date_unix                    | Number     |                                          |                       | Sí        |
| date_local                   | String     |                                          |                       | Sí        |
| date_precision               | String     | half, quarter, year, month, day, hour   |                       | Sí        |
| upcoming                     | Boolean    |                                          |                       | Sí        |
| static_fire_date_utc         | String     |                                          | null                  | No        |
| static_fire_date_unix        | Number     |                                          | null                  | No        |
| tdb                          | Boolean    |                                          | false                 | No        |
| net                          | Boolean    |                                          | false                 | No        |
| window                       | Number     |                                          | null                  | No        |
| rocket                       | UUID       |                                          | null                  | No        |
| success                      | Boolean    |                                          | null                  | No        |
| failures                     | Array[Object] |                                      |                       | No        |
|   - time                     | Number     |                                          |                       | No        |
|   - altitude                 | Number     |                                          |                       | No        |
|   - reason                   | String     |                                          |                       | No        |
| details                      | String     |                                          | null                  | No        |
| fairings                     | Object     |                                          |                       | No        |
|   - reused                   | Boolean    |                                          | null                  | No        |
|   - recovery_attempt         | Boolean    |                                          | null                  | No        |
|   - recovered                | Boolean    |                                          | null                  | No        |
|   - ships                    | Array[UUID] |                                      |                       | No        |
| crew                         | Array[UUID] |                                          |                       | No        |
| ships                        | Array[UUID] |                                          |                       | No        |
| capsules                     | Array[UUID] |                                          |                       | No        |
| payloads                     | Array[UUID] |                                          |                       | No        |
| launchpad                    | UUID       |                                          | null                  | No        |
| cores                        | Array[Object] |                                    |                       | No        |
|   - core                    | UUID       |                                          | null                  | No        |
|   - flight                  | Number     |                                          | null                  | No        |
|   - gridfins                | Boolean    |                                          | null                  | No        |
|   - legs                    | Boolean    |                                          | null                  | No        |
|   - reused                  | Boolean    |                                          | null                  | No        |
|   - landing_attempt         | Boolean    |                                          | null                  | No        |
|   - landing_success         | Boolean    |                                          | null                  | No        |
|   - landing_type            | String     |                                          | null                  | No        |
|   - landpad                 | UUID       |                                          | null                  | No        |
| links                        | Object     |                                          |                       | No        |
|   - patch                    | Object     |                                        |                       | No        |
|     - small                 | String     |                                          | null                  | No        |
|     - large                 | String     |                                          | null                  | No        |
|   - reddit                   | Object     |                                        |                       | No        |
|     - campaign              | String     |                                          | null                  | No        |
|     - launch                | String     |                                          | null                  | No        |
|     - media                 | String     |                                          | null                  | No        |
|     - recovery              | String     |                                          | null                  | No        |
|   - flickr                   | Object     |                                        |                       | No        |
|     - small                 | Array[String] |                                    |                       | No        |
|     - original              | Array[String] |                                    |                       | No        |
|   - presskit                 | String     |                                          | null                  | No        |
|   - webcast                  | String     |                                          | null                  | No        |
|   - youtube_id               | String     |                                          | null                  | No        |
|   - article                  | String     |                                          | null                  | No        |
|   - wikipedia                | String     |                                          | null                  | No        |
| auto_update                  | Boolean    |                                          | true                  | No        |

# Campos Rockets

**URL**: `https://api.spacexdata.com/v4/rockets`

| Campo                   | Tipo       | Valores Permitidos                | Valor Predeterminado | Requerido |
|-------------------------|------------|----------------------------------|-----------------------|-----------|
| name                    | String     |                                  |                       | No        |
| type                    | String     |                                  |                       | No        |
| active                  | Boolean    |                                  |                       | No        |
| stages                  | Number     |                                  |                       | No        |
| boosters                | Number     |                                  |                       | No        |
| cost_per_launch         | Number     |                                  |                       | No        |
| success_rate_pct       | Number     |                                  |                       | No        |
| first_flight            | String     |                                  |                       | No        |
| country                | String     |                                  |                       | No        |
| company                | String     |                                  |                       | No        |
| height                  |            |                                  |                       |           |
|   - meters             | Number     |                                  |                       | No        |
|   - feet               | Number     |                                  |                       | No        |
| diameter                |            |                                  |                       |           |
|   - meters             | Number     |                                  |                       | No        |
|   - feet               | Number     |                                  |                       | No        |
| mass                    |            |                                  |                       |           |
|   - kg                 | Number     |                                  |                       | No        |
|   - lb                 | Number     |                                  |                       | No        |
| payload_weights         | [Object]   |                                  |                       | No        |
| first_stage             |            |                                  |                       |           |
|   - reusable           | Boolean    |                                  |                       | No        |
|   - engines            | Number     |                                  |                       | No        |
|   - fuel_amount_tons   | Number     |                                  |                       | No        |
|   - burn_time_sec      | Number     |                                  |                       | No        |
|   - thrust_sea_level   |            |                                  |                       |           |
|     - kN               | Number     |                                  |                       | No        |
|     - lbf              | Number     |                                  |                       | No        |
|   - thrust_vacuum      |            |                                  |                       |           |
|     - kN               | Number     |                                  |                       | No        |
|     - lbf              | Number     |                                  |                       | No        |
| second_stage            |            |                                  |                       |           |
|   - reusable           | Boolean    |                                  |                       | No        |
|   - engines            | Number     |                                  |                       | No        |
|   - fuel_amount_tons   | Number     |                                  |                       | No        |
|   - burn_time_sec      | Number     |                                  |                       | No        |
|   - thrust             |            |                                  |                       |           |
|     - kN               | Number     |                                  |                       | No        |
|     - lbf              | Number     |                                  |                       | No        |
|   - payloads           |            |                                  |                       |           |
|     - option_1         | String     |                                  |                       | No        |
|     - composite_fairing|            |                                  |                       |           |
|       - height          |            |                                  |                       |           |
|         - meters        | Number     |                                  |                       | No        |
|         - feet          | Number     |                                  |                       | No        |
|       - diameter        |            |                                  |                       |           |
|         - meters        | Number     |                                  |                       | No        |
|         - feet          | Number     |                                  |                       | No        |
| engines                 |            |                                  |                       |           |
|   - number              | Number     |                                  |                       | No        |
|   - type                | String     |                                  |                       | No        |
|   - version             | String     |                                  |                       | No        |
|   - layout              | String     |                                  |                       | No        |
|   - isp                 |            |                                  |                       |           |
|     - sea_level         | Number     |                                  |                       | No        |
|     - vacuum            | Number     |                                  |                       | No        |
|   - engine_loss_max     | Number     |                                  |                       | No        |
|   - propellant_1        | String     |                                  |                       | No        |
|   - propellant_2        | String     |                                  |                       | No        |
|   - thrust_sea_level    |            |                                  |                       |           |
|     - kN               | Number     |                                  |                       | No        |
|     - lbf              | Number     |                                  |                       | No        |
|  

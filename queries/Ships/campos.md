# Campos Ships

**URL**: `https://api.spacexdata.com/v4/ships`

| Campo             | Tipo     | Valores Permitidos | Valor Predeterminado | Requerido |
|-------------------|----------|--------------------|-----------------------|-----------|
| name              | String   |                    |                       | Sí        |
| legacy_id         | String   |                    |                       | No        |
| model             | String   |                    |                       | No        |
| type              | String   |                    |                       | No        |
| roles             | [String] |                    |                       | No        |
| active            | Boolean  |                    |                       | Sí        |
| imo               | Number   |                    |                       | No        |
| mmsi              | Number   |                    |                       | No        |
| abs               | Number   |                    |                       | No        |
| class             | Number   |                    |                       | No        |
| mass_kg           | Number   |                    |                       | No        |
| mass_lbs          | Number   |                    |                       | No        |
| year_built        | Number   |                    |                       | No        |
| home_port         | String   |                    |                       | No        |
| status            | String   |                    |                       | No        |
| speed_kn          | Number   |                    |                       | No        |
| course_deg        | Number   |                    |                       | No        |
| latitude          | Number   |                    |                       | No        |
| longitude         | Number   |                    |                       | No        |
| last_ais_update   | String   |                    |                       | No        |
| link              | String   |                    |                       | No        |
| image             | String   |                    |                       | No        |
| launches          |          |                    |                       |           |
|   - type          | UUID     |                    |                       | No        |

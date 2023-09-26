# Campos Capsules

**URL** : `https://api.spacexdata.com/v4/capsules`

| Campo          | Tipo     | Valores Posibles                          | Requerido | Único | Valor Predeterminado |
|----------------|----------|------------------------------------------|-----------|-------|----------------------|
| serial         | String   | -                                        | Sí        | Sí    | -                    |
| status         | String   | "unknown", "active", "retired", "destroyed" | Sí        | No    | -                    |
| type           | String   | "Dragon 1.0", "Dragon 1.1", "Dragon 2.0"   | Sí        | No    | -                    |
| dragon         | UUID     | -                                        | No        | No    | -                    |
| reuse_count    | Number   | -                                        | No        | No    | 0                    |
| water_landings | Number   | -                                        | No        | No    | 0                    |
| land_landings  | Number   | -                                        | No        | No    | 0                    |
| last_update    | String   | -                                        | No        | No    | null                 |
| launches       | UUID[]   | -                                        | No        | No    | -                    |
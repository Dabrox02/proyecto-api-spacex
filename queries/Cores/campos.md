# Campos Cores

**URL**:`https://api.spacexdata.com/v4/cores`

| Campo          | Tipo   | Valores Permitidos                                        | Valor Predeterminado | Requerido |
|----------------|--------|----------------------------------------------------------|-----------------------|-----------|
| serial         | String |                                                          |                       | Sí        |
| block          | Number |                                                          | null                  | No        |
| status         | String | active, inactive, unknown, expended, lost, retired       |                       | Sí        |
| reuse_count    | Number |                                                          | 0                     | No        |
| rtls_attempts  | Number |                                                          | 0                     | No        |
| rtls_landings  | Number |                                                          | 0                     | No        |
| asds_attempts  | Number |                                                          | 0                     | No        |
| asds_landings  | Number |                                                          | 0                     | No        |
| last_update    | String |                                                          | null                  | No        |
| launches       | Array  |                                                          |                       | No        |

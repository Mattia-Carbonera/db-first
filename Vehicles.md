# Vehicles tab

| name                   | type          | attribute                           | key     | note                                                       |
| ---------------------- | ------------- | ----------------------------------- | ------- | ---------------------------------------------------------- |
| id                     | BIGINT(20)    | NOT NULL - AUTOINCREMENT - UNSIGNED | PRIMARY |                                                            |
| VIN                    | CHAR(17)      | NOT NULL - UNIQUE                   |         | Vehicle Identification Number: codice univoco 17 caratteri |
| brand                  | VARCHAR(20)   | NOT NULL                            |         |                                                            |
| model                  | VARCHAR(80)   |                                     |         |                                                            |
| color                  | VARCHAR(25)   |                                     |         |                                                            |
| seats                  | SMALLINT      | UNSIGNED                            |         |                                                            |
| conutry                | VARCHAR(3)    | NOT NULL - DEFAULT("IT")            |         | Paese di provenienza del veicolo come da targa             |
| condition              | CHAR(1)       |                                     |         | G => good, M => medium, B => bad                           |
| manufacrured_at        | YEAR          |                                     |         |                                                            |
| last_car_inspection_at | DATE          | NULL                                |         |                                                            |
| past-owners            | SMALLINT      | UNSIGNED                            |         |                                                            |
| price                  | DECIMAL(10,2) | UNSIGNED                            |         |                                                            |

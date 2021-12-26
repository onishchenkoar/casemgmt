# SUBJSRCH_CONFIG_MASTER

---

SUBJSRCH_CONFIG_MASTER This table is used to configure the match criteria for subject search. Subjects are considered as 'matched' when one or many of these match criteria are met.

[Back to index](./index.md)

| Column Name          | Data Type     | Column Null Option   | Column Definition                                                                                                                                                                                                                                                                  |
|:---------------------|:--------------|:---------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| SUBJSRCH_CONFIG_RK   | NUMBER(10)    | Not Null             | Since source data for SUBJSRCH_CONFIG_MASTER may come from multiple systems, the business supplied keys may not be unique. A surrogate key is added in the ETL process to ensure a unique identifier for SUBJSRCH_CONFIG_MASTER. Used with valid_from_dttm for versioning of rows. |
| SUBJSRCH_CONFIG_ID   | VARCHAR2(32)  | Not Null             | ID of the Case Network Analysis match criterion.                                                                                                                                                                                                                                   |
| SUBJSRCH_CONFIG_DESC | VARCHAR2(100) | Null                 | Description of the Case Network Analysis match criterion.                                                                                                                                                                                                                          |
| DELETE_FLG           | CHAR(1)       | Not Null             | Has the record been logically deleted?                                                                                                                                                                                                                                             |
| CREATE_USER_ID       | VARCHAR2(60)  | Null                 | Id of the user who created the Related Item Config record.                                                                                                                                                                                                                         |
| CREATE_DTTM          | TIMESTAMP     | Null                 | Date and time of when record was added.                                                                                                                                                                                                                                            |
| UPDATE_USER_ID       | VARCHAR2(60)  | Null                 | ID of the user who updated this record.                                                                                                                                                                                                                                            |

[Back to index](./index.md)
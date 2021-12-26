# RELATED_ITEM_CONFIG

---

This table is used to define different scenarios to find related incidents, cases and parties.

[Back to index](./index.md)

| Column Name               | Data Type     | Column Null Option   | Column Definition                                                                                                                                                                                                                                                            |
|:--------------------------|:--------------|:---------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RELATED_ITEM_RK           | NUMBER(10)    | Not Null             | Since source data for RELATED_ITEM_CONFIG may come from multiple systems, the business supplied keys may not be unique. A surrogate key is added in the ETL process to ensure a unique identifier for RELATED_ITEM_CONFIG. Used with valid_from_dttm for versioning of rows. |
| RELATED_ITEM_ID           | VARCHAR2(32)  | Not Null             | Related Item ID.                                                                                                                                                                                                                                                             |
| RELATED_ITEM_DESC         | VARCHAR2(100) | Null                 | Description field.                                                                                                                                                                                                                                                           |
| RELATED_PARTY_FIELD_NM    | VARCHAR2(30)  | Null                 | Name of the subject field that will be used to match the subjects.                                                                                                                                                                                                           |
| RELATED_INCIDENT_FIELD_NM | VARCHAR2(30)  | Null                 | Name of the incident field that will be used to match incidents.                                                                                                                                                                                                             |
| RELATED_CASE_FIELD_NM     | VARCHAR2(30)  | Null                 | Name of the case field that will be used to match the cases.                                                                                                                                                                                                                 |
| CREATE_USER_ID            | VARCHAR2(60)  | Null                 | ID of the user who created the Related Item Config record.                                                                                                                                                                                                                   |
| CREATE_DTTM               | TIMESTAMP     | Null                 | Date and time of when record was added.                                                                                                                                                                                                                                      |
| UPDATE_USER_ID            | VARCHAR2(60)  | Null                 | ID of the user who updated this record.                                                                                                                                                                                                                                      |
| DELETE_FLG                | CHAR(1)       | Not Null             | Has the record been logically deleted?                                                                                                                                                                                                                                       |

[Back to index](./index.md)
# SNA_CONFIG_DETAIL

---

This table stores the detail definition of SNA_CONFIG_MASTER. It contains one or many records of each SNA_CONFIG_MASTER record. A SNA_CONFIG_MASTER match criterion is considered as met when all of its associated SNA_CONFIG_DETAIL match criteria are met.

[Back to index](./index.md)

| Column Name          | Data Type      | Column Null Option   | Column Definition                                                                                                                                                                                                                                                        |
|:---------------------|:---------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| SNA_CONFIG_RK        | NUMBER(10)     | Not Null             | Since source data for SNA_CONFIG_DETAIL may come from multiple systems, the business supplied keys may not be unique. A surrogate key is added in the ETL process to ensure a unique identifier for SNA_CONFIG_DETAIL. Used with valid_from_dttm for versioning of rows. |
| SNA_CONFIG_SEQ_NO    | NUMBER(10)     | Not Null             | System generated sequence. The combination of SNA_CONFIG_RK and SNA_CONFIG_SEQ_NO make the record unique.                                                                                                                                                                |
| FROM_PARTY_TABLE_NM  | VARCHAR2(30)   | Null                 | Name of the table where FROM_PARTY_FIELD_NM is found                                                                                                                                                                                                                     |
| FROM_PARTY_FIELD_NM  | VARCHAR2(30)   | Null                 | Name of the subject form matching subjects. This is the 'match from' field.                                                                                                                                                                                              |
| FROM_PARTY_FIELD_EXP | VARCHAR2(4000) | Null                 | Expression to be used to define FROM_PARTY_FIELD_NM. If blank, FROM_PARTY_FIELD_NM will be used for matching subjects.                                                                                                                                                   |
| TO_PARTY_TABLE_NM    | VARCHAR2(30)   | Null                 | Name of the table where TO_PARTY_FIELD_NM is found                                                                                                                                                                                                                       |
| TO_PARTY_FIELD_NM    | VARCHAR2(30)   | Null                 | Name of the subject field for matching subjects. This is the 'match to' field.                                                                                                                                                                                           |
| TO_PARTY_FIELD_EXP   | VARCHAR2(4000) | Null                 | Expression to be used to define TO_PARTY_FIELD_NM. If blank, TO_PARTY_FIELD_NM will be used for matching subjects                                                                                                                                                        |
| DELETE_FLG           | CHAR(1)        | Not Null             | Has the record been logically deleted?                                                                                                                                                                                                                                   |

[Back to index](./index.md)
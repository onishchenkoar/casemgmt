# GENERIC_DATA_UDF_CHAR_VALUE

---

Contains character data types for generic user defined values.

[Back to index](./index.md)

| Column Name     | Data Type      | Column Null Option   | Column Definition                                                                                                                                                                                                                                                                            |
|:----------------|:---------------|:---------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GENERIC_DATA_RK | NUMBER(10)     | Not Null             | Since source data for GENERIC_DATA_UDF_CHAR_VALUE may come from multiple systems, the business supplied keys may not be unique. A surrogate key is added in the ETL process to ensure a unique identifier for GENERIC_DATA_UDF_CHAR_VALUE. Used with valid_from_dttm for versioning of rows. |
| VALID_FROM_DTTM | TIMESTAMP      | Not Null             | Standard dates used for versioning. The row content is valid within the time range specified by FROM and TO dates. For a given identifier, versions of its rows are distinguished by different non-overlapping FROM and TO date ranges.                                                      |
| UDF_TABLE_NM    | VARCHAR2(30)   | Not Null             | User-defined field table name.                                                                                                                                                                                                                                                               |
| UDF_NM          | VARCHAR2(30)   | Not Null             | User-defined field name.                                                                                                                                                                                                                                                                     |
| VALID_TO_DTTM   | TIMESTAMP      | Null                 | Standard dates used for versioning. The row content is valid within the time range specified by FROM and TO dates. For a given identifier, versions of its rows are distinguished by different non-overlapping FROM and TO date ranges.                                                      |
| UDF_VALUE       | VARCHAR2(4000) | Not Null             | User-defined field value.                                                                                                                                                                                                                                                                    |

[Back to index](./index.md)
# GENERIC_DATA_UDF_NUM_VALUE

---

Contains number data types for generic user defined values.

[Back to index](./index.md)

| Column Name     | Data Type        | Column Null Option   | Column Definition                                                                                                                                                                                                                       |
|:----------------|:-----------------|:---------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| VALID_FROM_DTTM | TIMESTAMP        | Not Null             | Standard dates used for versioning. The row content is valid within the time range specified by FROM and TO dates. For a given identifier, versions of its rows are distinguished by different non-overlapping FROM and TO date ranges. |
| UDF_TABLE_NM    | VARCHAR2(30)     | Not Null             | User-defined field table name.                                                                                                                                                                                                          |
| UDF_NM          | VARCHAR2(30)     | Not Null             | User-defined field name.                                                                                                                                                                                                                |
| VALID_TO_DTTM   | TIMESTAMP        | Null                 | Standard dates used for versioning. The row content is valid within the time range specified by FROM and TO dates. For a given identifier, versions of its rows are distinguished by different non-overlapping FROM and TO date ranges. |
| UDF_VALUE       | DOUBLE PRECISION | Not Null             | User-defined field value.                                                                                                                                                                                                               |

[Back to index](./index.md)
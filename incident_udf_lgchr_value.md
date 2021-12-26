# INCIDENT_UDF_LGCHR_VALUE

---

Contains CLOB or long character data typed user defined field values for incidents.

[Back to index](./index.md)

| Column Name     | Data Type    | Column Null Option   | Column Definition                                                                                                                                                                                                                       |
|:----------------|:-------------|:---------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| INCIDENT_RK     | NUMBER(10)   | Not Null             | System-generated incident surrogate key.                                                                                                                                                                                                |
| VALID_FROM_DTTM | TIMESTAMP    | Not Null             | Standard dates used for versioning. The row content is valid within the time range specified by FROM and TO dates. For a given identifier, versions of its rows are distinguished by different non-overlapping FROM and TO date ranges. |
| UDF_TABLE_NM    | VARCHAR2(30) | Not Null             | User-defined field table name.                                                                                                                                                                                                          |
| UDF_NM          | VARCHAR2(30) | Not Null             | User-defined field name.                                                                                                                                                                                                                |
| ROW_NO          | NUMBER(10)   | Not Null             | Row number.                                                                                                                                                                                                                             |
| UDF_VALUE       | CLOB         | Null                 | User-defined field value.                                                                                                                                                                                                               |

[Back to index](./index.md)
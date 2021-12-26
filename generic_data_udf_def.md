# GENERIC_DATA_UDF_DEF

---

Details of user defined field definitions for a generic item.

[Back to index](./index.md)

| Column Name   | Data Type     | Column Null Option   | Column Definition                                                                 |
|:--------------|:--------------|:---------------------|:----------------------------------------------------------------------------------|
| UDF_TABLE_NM  | VARCHAR2(30)  | Not Null             | User-defined field table name.                                                    |
| UDF_NM        | VARCHAR2(30)  | Not Null             | User-defined field name.                                                          |
| UDF_TYPE_NM   | VARCHAR2(10)  | Not Null             | User-defined field data type (VARCHAR, BIGINT, DOUBLE, BOOLEAN, DATE, TIMESTAMP). |
| UDF_DESC      | VARCHAR2(100) | Null                 | User-defined field description.                                                   |
| MAX_CHAR_CNT  | NUMBER(6)     | Null                 | Maximum number of characters for a CHAR data typed user-defined field.            |
| REF_TABLE_NM  | VARCHAR2(30)  | Null                 | The name of the (optional) reference table used to display values for this field. |

[Back to index](./index.md)
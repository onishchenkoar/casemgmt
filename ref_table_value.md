# REF_TABLE_VALUE

---

Contains code value definitions for reference tables.

[Back to index](./index.md)

| Column Name         | Data Type     | Column Null Option   | Column Definition                                                 |
|:--------------------|:--------------|:---------------------|:------------------------------------------------------------------|
| VALUE_CD            | VARCHAR2(32)  | Not Null             | Coded value.                                                      |
| VALUE_DESC          | VARCHAR2(100) | Not Null             | Displayable value.                                                |
| PARENT_REF_TABLE_NM | VARCHAR2(30)  | Null                 | Reference table name.                                             |
| PARENT_VALUE_CD     | VARCHAR2(32)  | Null                 | Coded value.                                                      |
| DISPLAY_ORDER_NO    | NUMBER(6)     | Not Null             | Display order number.                                             |
| ACTIVE_FLG          | CHAR(1)       | Not Null             | Flag indicates whether the reference table value is still active. |

[Back to index](./index.md)
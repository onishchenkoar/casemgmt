# RR_SEARCH_FILTER_FIELD

---

Contains search filter field configurations for the case search screen.

[Back to index](./index.md)

| Column Name      | Data Type    | Column Null Option   | Column Definition                                                                               |
|:-----------------|:-------------|:---------------------|:------------------------------------------------------------------------------------------------|
| USER_ID          | VARCHAR2(60) | Not Null             | User who this configuration applies to. Equals '*' for the default configuration for all users. |
| TABLE_NM         | VARCHAR2(30) | Not Null             | Field table name.                                                                               |
| FIELD_NM         | VARCHAR2(30) | Not Null             | Field name.                                                                                     |
| DISPLAY_ORDER_NO | NUMBER(6)    | Not Null             | Display order number.                                                                           |
| REF_TABLE_NM     | VARCHAR2(30) | Not Null             | Reference table name to render a selection list filter for the field.                           |

[Back to index](./index.md)
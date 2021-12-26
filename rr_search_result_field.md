# RR_SEARCH_RESULT_FIELD

---

Contains search result field configurations for the case search screen.

[Back to index](./index.md)

| Column Name      | Data Type    | Column Null Option   | Column Definition                                                                                                                                                                                                                                                                                                                                                  |
|:-----------------|:-------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| DISPLAY_ORDER_NO | NUMBER(6)    | Not Null             | Display order number.                                                                                                                                                                                                                                                                                                                                              |
| REF_TABLE_NM     | VARCHAR2(30) | Null                 | Reference table name to render coded values as displayable values.                                                                                                                                                                                                                                                                                                 |
| FORMAT_TXT       | VARCHAR2(40) | Null                 | Contains one of two values: 1) A user_name - In this case the column is expected to be a user id, and that user's display name is looked up and rendered. 2) A number format understood by the java.text.DecimalFormat class. If this column contains a number format and the field type is BIGINT or DOUBLE, the number format is used to render the field value. |

[Back to index](./index.md)
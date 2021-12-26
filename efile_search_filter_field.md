# EFILE_SEARCH_FILTER_FIELD

---

Contains search filter field configurations for the case search screen.

[Back to index](./index.md)

| Column Name      | Data Type    | Column Null Option   | Column Definition                                                                               |
|:-----------------|:-------------|:---------------------|:------------------------------------------------------------------------------------------------|
| USER_ID          | VARCHAR2(60) | Not Null             | User who this configuration applies to. Equals '*' for the default configuration for all users. |
| TABLE_NM         | VARCHAR2(30) | Not Null             | Table name of field that can be used for filtering e-files.                                     |
| FIELD_NM         | VARCHAR2(30) | Not Null             | Field name of the field that can be used for filtering e-files.                                 |
| DISPLAY_ORDER_NO | NUMBER(6)    | Not Null             | Order number for displaying the search fields in the e-file filter UI.                          |
| REF_TABLE_NM     | VARCHAR2(30) | Not Null             | Reference table name to render a selection list filter for the field.                           |

[Back to index](./index.md)
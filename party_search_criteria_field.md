# PARTY_SEARCH_CRITERIA_FIELD

---

Contains search criteria field configurations for the party search screen.

[Back to index](./index.md)

| Column Name      | Data Type    | Column Null Option   | Column Definition                                                                               |
|:-----------------|:-------------|:---------------------|:------------------------------------------------------------------------------------------------|
| USER_ID          | VARCHAR2(60) | Not Null             | User who this configuration applies to. Equals '*' for the default configuration for all users. |
| TABLE_NM         | VARCHAR2(30) | Not Null             | Field table name.                                                                               |
| FIELD_NM         | VARCHAR2(30) | Not Null             | Field name.                                                                                     |
| DISPLAY_ORDER_NO | NUMBER(6)    | Not Null             | Display order number.                                                                           |
| REF_TABLE_NM     | VARCHAR2(30) | Null                 | Reference table name to render a selection list criteria filter for the field.                  |
| FORMAT_TXT       | VARCHAR2(40) | Null                 | Name of the resource bundle key that contains the display format for numeric fields.            |

[Back to index](./index.md)
# PARTY_CONFIG

---

Defines the rules which determine the ui definition to display for a given party, based on the party's type, category and subcategory values. If a record includes null for category or subcategory, that is treated as a wildcard and that rule would apply for any value in that column. In situations where multiple rules apply, the sequence number is treated as the priority; the matching rule with the smallest sequence number will be selected.

[Back to index](./index.md)

| Column Name          | Data Type     | Column Null Option   | Column Definition                                                                                                                                                                                                                    |
|:---------------------|:--------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| PARTY_CONFIG_SEQ_NO  | NUMBER(10)    | Not Null             | Party configuration sequence number. The sequence number is also used as a priority when multiple configurations apply for a given party. If multiple configurations apply, the one with the smaller sequence number will be chosen. |
| PARTY_TYPE_CD        | VARCHAR2(32)  | Not Null             | Party type code.                                                                                                                                                                                                                     |
| PARTY_CATEGORY_CD    | VARCHAR2(32)  | Null                 | Party category code.                                                                                                                                                                                                                 |
| PARTY_SUBCATEGORY_CD | VARCHAR2(32)  | Null                 | Party sub-category code.                                                                                                                                                                                                             |
| UI_DEF_FILE_NM       | VARCHAR2(100) | Not Null             | Custom Page Builder user interface definition file name.                                                                                                                                                                             |

[Back to index](./index.md)
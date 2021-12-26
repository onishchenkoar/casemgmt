# CASE_CONFIG

---

Defines the rules which determine the ui definition to display for a given case, based on the case type, category and subcategory values. If a record includes null for category or subcategory, that is treated as a wildcard and that rule would apply for any value in that column. In situations where multiple rules apply, the sequence number is treated as the priority; the matching rule with the smallest sequence number will be selected.

[Back to index](./index.md)

| Column Name                 | Data Type     | Column Null Option   | Column Definition                          |
|:----------------------------|:--------------|:---------------------|:-------------------------------------------|
| CASE_CONFIG_SEQ_NO          | NUMBER(10)    | Not Null             | Case sequence number.                      |
| CASE_TYPE_CD                | VARCHAR2(32)  | Not Null             | Case type code.                            |
| CASE_CATEGORY_CD            | VARCHAR2(32)  | Null                 | Case category code.                        |
| CASE_SUBCATEGORY_CD         | VARCHAR2(32)  | Null                 | Case subcategory code.                     |
| UI_DEF_FILE_NM              | VARCHAR2(100) | Not Null             | User interface definition file name.       |
| INVESTIGATE_WORKFLOW_DEF_NM | VARCHAR2(100) | Not Null             | Investigate case workflow definition name. |
| REOPEN_WORKFLOW_DEF_NM      | VARCHAR2(100) | Null                 | Reopen case workflow definition name.      |
| INVESTIGATOR_USER_ID        | VARCHAR2(60)  | Null                 | Investigator who initially owns the case.  |

[Back to index](./index.md)
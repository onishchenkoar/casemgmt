# RR_CONFIG

---

Defines the rules which determine the ui definition to display for a given report, based on the report's type, category and subcategory values. If a record includes null for category or subcategory, that is treated as a wildcard and that rule would apply for any value in that column. In situations where multiple rules apply, the sequence number is treated as the priority; the matching rule with the smallest sequence number will be selected.

[Back to index](./index.md)

| Column Name         | Data Type     | Column Null Option   | Column Definition                                                                                                                                                                                                                                        |
|:--------------------|:--------------|:---------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RR_CATEGORY_CD      | VARCHAR2(32)  | Null                 | Report category code.                                                                                                                                                                                                                                    |
| RR_SUBCATEGORY_CD   | VARCHAR2(32)  | Null                 | Report subcategory code.                                                                                                                                                                                                                                 |
| UI_DEF_FILE_NM      | VARCHAR2(100) | Not Null             | User interface definition file name.                                                                                                                                                                                                                     |
| FORM_AGENCY_CD      | VARCHAR2(32)  | Not Null             | Unique code to define the government agency who published the form.                                                                                                                                                                                      |
| FORM_TYPE_CD        | VARCHAR2(32)  | Not Null             | Unique code to define the government form published by the agency defined in FORM_AGENCY_CD.                                                                                                                                                             |
| EFILE_CONFIG_SEQ_NO | NUMBER(10)    | Null                 | Since source data for RR_CONFIG may come from multiple systems, the business supplied keys may not be unique. A surrogate key is added in the ETL process to ensure a unique identifier for RR_CONFIG. Used with valid_from_dttm for versioning of rows. |
| WORKFLOW_DEF_NM     | VARCHAR2(100) | Null                 | Report workflow definition name.                                                                                                                                                                                                                         |

[Back to index](./index.md)
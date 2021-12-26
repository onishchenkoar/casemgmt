# CASE_LIVE

---

Details of a case involving one or more suspicious incidents. This table contains the current version of the Case.

[Back to index](./index.md)

| Column Name            | Data Type     | Column Null Option   | Column Definition                                                                           |
|:-----------------------|:--------------|:---------------------|:--------------------------------------------------------------------------------------------|
| CASE_TYPE_CD           | VARCHAR2(32)  | Null                 | Case type code.                                                                             |
| CASE_CATEGORY_CD       | VARCHAR2(32)  | Null                 | Case category code.                                                                         |
| CASE_SUBCATEGORY_CD    | VARCHAR2(32)  | Null                 | Case sub-category code.                                                                     |
| CASE_STATUS_CD         | VARCHAR2(10)  | Null                 | Case status code.                                                                           |
| CASE_DISPOSITION_CD    | VARCHAR2(10)  | Null                 | Case disposition code.                                                                      |
| CASE_DESC              | VARCHAR2(100) | Null                 | Case description.                                                                           |
| CASE_LINK_SK           | NUMBER(10)    | Null                 | System generated surrogate key for linking related cases.                                   |
| PRIORITY_CD            | VARCHAR2(10)  | Null                 | The priority code of a case is used for sorting (for example, High, Medium, and Low).       |
| REGULATORY_RPT_RQD_FLG | CHAR(1)       | Not Null             | Regulatory report required flag.                                                            |
| INVESTIGATOR_USER_ID   | VARCHAR2(60)  | Null                 | Investigator who owns the case.                                                             |
| OPEN_DTTM              | TIMESTAMP     | Null                 | Date and time when the cae was opened.                                                      |
| REOPEN_DTTM            | TIMESTAMP     | Null                 | Date and time when the case was last re-opened.                                             |
| CLOSE_DTTM             | TIMESTAMP     | Null                 | Date and time when the case was closed.                                                     |
| UI_DEF_FILE_NM         | VARCHAR2(100) | Null                 | Custom Page Builder user interface file name.                                               |
| CREATE_USER_ID         | VARCHAR2(60)  | Null                 | User who created the case.                                                                  |
| CREATE_DTTM            | TIMESTAMP     | Not Null             | Date and time when the case was created.                                                    |
| UPDATE_USER_ID         | VARCHAR2(60)  | Null                 | User who last updated the case.                                                             |
| VERSION_NO             | NUMBER(10)    | Not Null             | Version number used to implement optimistic locking.                                        |
| DELETE_FLG             | CHAR(1)       | Not Null             | This flag indicates whether or not the case has been logically deleted and is now obsolete. |

[Back to index](./index.md)
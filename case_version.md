# CASE_VERSION

---

Details of a case involving one or more suspicious incidents.

[Back to index](./index.md)

| Column Name    | Data Type     | Column Null Option   | Column Definition                                                                           |
|:---------------|:--------------|:---------------------|:--------------------------------------------------------------------------------------------|
| UI_DEF_FILE_NM | VARCHAR2(100) | Null                 | Custom Page Builder user interface file name.                                               |
| CREATE_USER_ID | VARCHAR2(60)  | Null                 | User who created the case.                                                                  |
| CREATE_DTTM    | TIMESTAMP     | Not Null             | Date and time when the case was created.                                                    |
| UPDATE_USER_ID | VARCHAR2(60)  | Null                 | User who last updated the case.                                                             |
| VERSION_NO     | NUMBER(10)    | Not Null             | Version number used to implement optimistic locking.                                        |
| DELETE_FLG     | CHAR(1)       | Not Null             | This flag indicates whether or not the Case has been logically deleted and is now obsolete. |

[Back to index](./index.md)
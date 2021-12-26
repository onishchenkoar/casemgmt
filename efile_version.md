# EFILE_VERSION

---

Details of an efile. This table contains all versions of the efile.

[Back to index](./index.md)

| Column Name    | Data Type     | Column Null Option   | Column Definition                               |
|:---------------|:--------------|:---------------------|:------------------------------------------------|
| OWNER_USER_ID  | VARCHAR2(60)  | Null                 | User who initially owns the report.             |
| UI_DEF_FILE_NM | VARCHAR2(100) | Null                 | User interface definition file name.            |
| CREATE_USER_ID | VARCHAR2(60)  | Null                 | The ID of the user that added the record.       |
| CREATE_DTTM    | TIMESTAMP     | Null                 | The date and time when the record was added.    |
| UPDATE_USER_ID | VARCHAR2(60)  | Null                 | The ID of the user who updated the record.      |
| VERSION_NO     | NUMBER(10)    | Not Null             | The date and time when the record was updated.  |
| DELETE_FLG     | CHAR(1)       | Not Null             | A flag indicating whether the record is active. |

[Back to index](./index.md)
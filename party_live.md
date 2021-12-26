# PARTY_LIVE

---

Details of an individual or organization that plays a role in a case or a suspicious incident. This table contains the current version of the Party.

[Back to index](./index.md)

| Column Name             | Data Type     | Column Null Option   | Column Definition                                                                            |
|:------------------------|:--------------|:---------------------|:---------------------------------------------------------------------------------------------|
| SOURCE_SYSTEM_CD        | VARCHAR2(10)  | Not Null             | Source system code.                                                                          |
| PARTY_TYPE_CD           | VARCHAR2(32)  | Null                 | Party type code.                                                                             |
| PARTY_CATEGORY_CD       | VARCHAR2(32)  | Null                 | Party category code.                                                                         |
| PARTY_SUBCATEGORY_CD    | VARCHAR2(32)  | Null                 | Party sub-category code.                                                                     |
| IDENTICAL_PARTY_LINK_SK | NUMBER(10)    | Null                 | System generated surrogate key for linking identical parties.                                |
| INDIVIDUAL_FLG          | CHAR(1)       | Not Null             | Is the party an individual?                                                                  |
| PARTY_FULL_NM           | VARCHAR2(200) | Null                 | Party full name.                                                                             |
| NATIONAL_ID             | VARCHAR2(32)  | Null                 | National identification number.                                                              |
| NATIONAL_ID_TYPE_CD     | VARCHAR2(10)  | Null                 | National identification number type code.                                                    |
| UI_DEF_FILE_NM          | VARCHAR2(100) | Null                 | Custom Page Builder user interface file name.                                                |
| CREATE_USER_ID          | VARCHAR2(60)  | Null                 | User who created the party.                                                                  |
| CREATE_DTTM             | TIMESTAMP     | Not Null             | Date and time when the party was created.                                                    |
| UPDATE_USER_ID          | VARCHAR2(60)  | Null                 | User who last updated the party.                                                             |
| VERSION_NO              | NUMBER(10)    | Not Null             | Version number used to implement optimistic locking.                                         |
| DELETE_FLG              | CHAR(1)       | Not Null             | This flag indicates whether or not the Party has been logically deleted and is now obsolete. |

[Back to index](./index.md)
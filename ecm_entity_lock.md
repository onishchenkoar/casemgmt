# ECM_ENTITY_LOCK

---

Allows any user-editable ECM object to be locked before editing.

[Back to index](./index.md)

| Column Name   | Data Type     | Column Null Option   | Column Definition                                                                                                                                                                                         |
|:--------------|:--------------|:---------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ENTITY_RK     | NUMBER(10)    | Not Null             | A sequential system generated key. A surrogate key is added in the ETL process to ensure a unique identifier. May be used with validity date ranges in order to establish historical changes in the data. |
| ENTITY_NM     | VARCHAR2(100) | Not Null             | Entity name.                                                                                                                                                                                              |
| LOCK_USER_ID  | VARCHAR2(60)  | Not Null             | User ID that is locking the SAS Enterprise Case Management object.                                                                                                                                        |
| LOCK_DTTM     | TIMESTAMP     | Not Null             | Date and time the lock on the object occurred.                                                                                                                                                            |

[Back to index](./index.md)
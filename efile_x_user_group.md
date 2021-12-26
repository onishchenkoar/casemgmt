# EFILE_X_USER_GROUP

---

Intersection table linking efiles to groups of users who can access the efile.

[Back to index](./index.md)

| Column Name   | Data Type    | Column Null Option   | Column Definition                                                                                                                                                                                                                                                          |
|:--------------|:-------------|:---------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| EFILE_RK      | NUMBER(10)   | Not Null             | Since source data for EFILE_X_USER_GROUP may come from multiple systems, the business supplied keys may not be unique. A surrogate key is added in the ETL process to ensure a unique identifier for EFILE_X_USER_GROUP. Used with valid_from_dttm for versioning of rows. |
| USER_GROUP_NM | VARCHAR2(60) | Not Null             | User group name.                                                                                                                                                                                                                                                           |

[Back to index](./index.md)
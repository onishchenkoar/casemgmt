# RR_X_USER_GROUP

---

Intersection table linking reports to groups of users who can access the report.

[Back to index](./index.md)

| Column Name   | Data Type    | Column Null Option   | Column Definition                                                                                                                                                                                                                                                    |
|:--------------|:-------------|:---------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RR_RK         | NUMBER(10)   | Not Null             | Since source data for RR_X_USER_GROUP may come from multiple systems, the business supplied keys may not be unique. A surrogate key is added in the ETL process to ensure a unique identifier for RR_X_USER_GROUP. Used with valid_from_dttm for versioning of rows. |
| USER_GROUP_NM | VARCHAR2(60) | Not Null             | User group name.                                                                                                                                                                                                                                                     |

[Back to index](./index.md)
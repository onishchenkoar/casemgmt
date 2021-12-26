# CASE_X_USER_GROUP

---

Intersection table linking cases to groups of users who can access the case.

[Back to index](./index.md)

| Column Name   | Data Type    | Column Null Option   | Column Definition                                            |
|:--------------|:-------------|:---------------------|:-------------------------------------------------------------|
| CASE_RK       | NUMBER(10)   | Not Null             | System generated case surrogate key.                         |
| USER_GROUP_NM | VARCHAR2(60) | Not Null             | User group name. Equals '*' if any user may access the case. |

[Back to index](./index.md)
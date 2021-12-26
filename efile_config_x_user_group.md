# EFILE_CONFIG_X_USER_GROUP

---

Intersection table linking the initial groups of users who can access an efile to an efile configuration

[Back to index](./index.md)

| Column Name         | Data Type    | Column Null Option   | Column Definition                                                      |
|:--------------------|:-------------|:---------------------|:-----------------------------------------------------------------------|
| EFILE_CONFIG_SEQ_NO | NUMBER(10)   | Not Null             | Key to link e-file configuration record to a user group.               |
| USER_GROUP_NM       | VARCHAR2(60) | Not Null             | Unique key to link the user group with an e-file configuration record. |

[Back to index](./index.md)
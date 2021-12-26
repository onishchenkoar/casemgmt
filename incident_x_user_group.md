# INCIDENT_X_USER_GROUP

---

Intersection table linking incidents to groups of users who can access the indicent.

[Back to index](./index.md)

| Column Name   | Data Type    | Column Null Option   | Column Definition                                                |
|:--------------|:-------------|:---------------------|:-----------------------------------------------------------------|
| INCIDENT_RK   | NUMBER(10)   | Not Null             | System-generated incident surrogate key.                         |
| USER_GROUP_NM | VARCHAR2(60) | Not Null             | User group name. Equals '*' if any user may access the incident. |

[Back to index](./index.md)
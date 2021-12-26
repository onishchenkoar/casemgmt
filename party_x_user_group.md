# PARTY_X_USER_GROUP

---

Intersection table linking parties to groups of users who can access the party.

[Back to index](./index.md)

| Column Name   | Data Type    | Column Null Option   | Column Definition                                             |
|:--------------|:-------------|:---------------------|:--------------------------------------------------------------|
| PARTY_RK      | NUMBER(10)   | Not Null             | System-generated party retained surrogate key.                |
| USER_GROUP_NM | VARCHAR2(60) | Not Null             | User group name. Equals '*' if any user may access the party. |

[Back to index](./index.md)
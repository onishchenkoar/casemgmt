# PARTY_X_PARTY

---

Intersection table linking parties to other parties.

[Back to index](./index.md)

| Column Name     | Data Type     | Column Null Option   | Column Definition                                           |
|:----------------|:--------------|:---------------------|:------------------------------------------------------------|
| PARTY_RK        | NUMBER(10)    | Not Null             | System-generated party retained surrogate key.              |
| MEMBER_PARTY_RK | NUMBER(10)    | Not Null             | Surrogate key of a party that is a member of another party. |
| MEMBER_TYPE_CD  | VARCHAR2(10)  | Not Null             | Membership type code.                                       |
| MEMBER_DESC     | VARCHAR2(100) | Null                 | Membership description.                                     |

[Back to index](./index.md)
# CASE_X_PARTY

---

Intersection table linking parties to cases.

[Back to index](./index.md)

| Column Name      | Data Type     | Column Null Option   | Column Definition                                               |
|:-----------------|:--------------|:---------------------|:----------------------------------------------------------------|
| CASE_RK          | NUMBER(10)    | Not Null             | System-generated case surrogate key.                            |
| PARTY_RK         | NUMBER(10)    | Not Null             | System-generated party retained surrogate key.                  |
| RELATION_TYPE_CD | VARCHAR2(10)  | Not Null             | Relationship type code.                                         |
| RELATION_DESC    | VARCHAR2(100) | Null                 | Relationship description.                                       |
| CREATE_DTTM      | TIMESTAMP     | Not Null             | Date and time when the case and party relationship was created. |

[Back to index](./index.md)
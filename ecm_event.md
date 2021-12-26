# ECM_EVENT

---

Consolidated audit trail table for all objects.

[Back to index](./index.md)

| Column Name        | Data Type     | Column Null Option   | Column Definition                                                                           |
|:-------------------|:--------------|:---------------------|:--------------------------------------------------------------------------------------------|
| EVENT_RK           | NUMBER(10)    | Not Null             | System generated event surrogate key.                                                       |
| BUSINESS_OBJECT_NM | VARCHAR2(100) | Not Null             | Name of the type of object this event is associated with: CASE, INCIDENT, PARTY, RR, EFILE. |
| BUSINESS_OBJECT_RK | NUMBER(10)    | Not Null             | Key value of the event that is associated with this object.                                 |
| EVENT_TYPE_CD      | VARCHAR2(10)  | Not Null             | Event type code.                                                                            |
| EVENT_DESC         | VARCHAR2(256) | Null                 | Event description.                                                                          |
| CREATE_USER_ID     | VARCHAR2(60)  | Null                 | User who created the event.                                                                 |
| CREATE_DTTM        | TIMESTAMP     | Not Null             | Date and time when the event was created.                                                   |
| LINKED_OBJECT_NM   | VARCHAR2(100) | Null                 | Linked object name.                                                                         |
| LINKED_OBJECT_RK   | NUMBER(10)    | Null                 | Linked object surrogate key.                                                                |

[Back to index](./index.md)
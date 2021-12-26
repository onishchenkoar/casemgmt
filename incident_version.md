# INCIDENT_VERSION

---

Details of a suspicious incident.

[Back to index](./index.md)

| Column Name             | Data Type     | Column Null Option   | Column Definition                                    |
|:------------------------|:--------------|:---------------------|:-----------------------------------------------------|
| SOURCE_SYSTEM_CD        | VARCHAR2(10)  | Not Null             | Source system code.                                  |
| INCIDENT_TYPE_CD        | VARCHAR2(32)  | Null                 | Incident type code.                                  |
| INCIDENT_CATEGORY_CD    | VARCHAR2(32)  | Null                 | Incident category code.                              |
| INCIDENT_SUBCATEGORY_CD | VARCHAR2(32)  | Null                 | Incident sub-category code.                          |
| INCIDENT_DESC           | VARCHAR2(100) | Null                 | Incident description.                                |
| INCIDENT_FROM_DT        | DATE          | Null                 | Incident start date.                                 |
| INCIDENT_FROM_TM        | char(8)       | Null                 | Incident start time (format = HH:MM:SS).             |
| INCIDENT_TO_DT          | DATE          | Null                 | Incident end date.                                   |
| INCIDENT_TO_TM          | char(8)       | Null                 | Incident end time (format = HH:MM:SS).               |
| DETECTION_DT            | DATE          | Null                 | Incident detection date.                             |
| DETECTION_TM            | char(8)       | Null                 | Incident detection time (format = HH:MM:SS).         |
| NOTIFICATION_DT         | DATE          | Null                 | Incident notification date.                          |
| NOTIFICATION_TM         | char(8)       | Null                 | Incident notification time (format = HH:MM:SS).      |
| UI_DEF_FILE_NM          | VARCHAR2(100) | Null                 | Custom Page Builder user interface file name.        |
| CREATE_USER_ID          | VARCHAR2(60)  | Null                 | User who created the incident.                       |
| CREATE_DTTM             | TIMESTAMP     | Not Null             | Date and time when the incident was created.         |
| UPDATE_USER_ID          | VARCHAR2(60)  | Null                 | User who last updated the incident.                  |
| VERSION_NO              | NUMBER(10)    | Not Null             | Version number used to implement optimistic locking. |
| DELETE_FLG              | char(1)       | Not Null             | Has the incident been logically deleted?             |
| INVESTIGATOR_USER_ID    | VARCHAR2(60)  | Null                 | Investigator for the incident.                       |
| INCIDENT_DISPOSITION_CD | VARCHAR2(10)  | Null                 | Incident disposition code.                           |
| CLOSE_DTTM              | TIMESTAMP     | Null                 | Date and time when the incident was closed.          |
| INCIDENT_STATUS_CD      | VARCHAR2(10)  | Null                 | Incident status code.                                |

[Back to index](./index.md)
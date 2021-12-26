# TASK_LIST

---

Stores task list information related to a Case or an Incident with automatic reminders.

[Back to index](./index.md)

| Column Name        | Data Type      | Column Null Option   | Column Definition                                                                                                                                                                                                                                        |
|:-------------------|:---------------|:---------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| TASK_LIST_RK       | NUMBER(10)     | Not Null             | Since source data for TASK_LIST may come from multiple systems, the business supplied keys may not be unique. A surrogate key is added in the ETL process to ensure a unique identifier for TASK_LIST. Used with valid_from_dttm for versioning of rows. |
| BUSINESS_OBJECT_RK | NUMBER(10)     | Null                 | This key links the task to a case or an incident.                                                                                                                                                                                                        |
| BUSINESS_OBJECT_NM | VARCHAR2(100)  | Not Null             | The business object name links a Task to a Case or an Incident along with the surrogate key of that business object.                                                                                                                                     |
| TASK_DESC          | VARCHAR2(1000) | Not Null             | The description of the task.                                                                                                                                                                                                                             |
| TASK_GOAL_DT       | DATE           | Null                 | The expected completion date for this task.                                                                                                                                                                                                              |
| COMPLETE_FLG       | CHAR(1)        | Null                 | Is this task complete?                                                                                                                                                                                                                                   |
| TIMEZONE_OFFSET    | NUMBER         | Null                 | The time zone offset for the user who is to receive or who has received the reminder.                                                                                                                                                                    |
| REMINDER_DTTM      | TIMESTAMP      | Null                 | Standard dates used for versioning. The row content is valid within the time range specified by FROM and TO dates. For a given identifier, versions of its rows are distinguished by different non-overlapping FROM and TO date ranges.                  |
| REMINDER_SENT_DTTM | TIMESTAMP      | Null                 | Standard dates used for versioning. The row content is valid within the time range specified by FROM and TO dates. For a given identifier, versions of its rows are distinguished by different non-overlapping FROM and TO date ranges.                  |
| OWNER_ID           | VARCHAR2(60)   | Null                 | The user ID of the current task owner.                                                                                                                                                                                                                   |
| REMINDER_USER_ID   | VARCHAR2(60)   | Null                 | The user ID of the reminder receipient.                                                                                                                                                                                                                  |
| ALERT_ID           | NUMBER(20)     | Null                 | The alert ID for the reminder to be issued.                                                                                                                                                                                                              |

[Back to index](./index.md)
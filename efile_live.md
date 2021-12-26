# EFILE_LIVE

---

Details of an efile. This table contains the current version of the efile.

[Back to index](./index.md)

| Column Name            | Data Type     | Column Null Option   | Column Definition                                                                                                               |
|:-----------------------|:--------------|:---------------------|:--------------------------------------------------------------------------------------------------------------------------------|
| EFILE_STATUS_CD        | VARCHAR2(10)  | Null                 | E-file status code, such as A for accepted and R for Rejected.                                                                  |
| EFILE_DESC             | VARCHAR2(100) | Null                 | Description of the e-file entered by the user or set by the batch program.                                                      |
| OUTPUT_PATH_NM         | VARCHAR2(100) | Null                 | Subdirectory where the output e-file is stored.                                                                                 |
| OUTPUT_NM              | VARCHAR2(100) | Null                 | Name of the output e-file.                                                                                                      |
| OUTPUT_RR_CNT          | NUMBER(10)    | Null                 | Number of reports in the output e-file.                                                                                         |
| OUTPUT_LINE_CNT        | NUMBER(10)    | Null                 | Number of lines in the output e-file.                                                                                           |
| OUTPUT_FILE_SIZE       | NUMBER(10)    | Null                 | Size of the output e-file.                                                                                                      |
| OUTPUT_CREATE_DTTM     | TIMESTAMP     | Null                 | Date and time when the output is created.                                                                                       |
| TRANSMISSION_ID        | VARCHAR2(100) | Null                 | Transmission ID provided by the agency after an e-file is submitted.                                                            |
| TRANSMISSION_DTTM      | TIMESTAMP     | Null                 | Date and time when the e-file was transmitted.                                                                                  |
| EFILE_AGENCY_REF_ID    | VARCHAR2(100) | Null                 | The reference ID provided by the agency to identify an accepted Efile. It is equivalent to Document Control Number from FINCEN. |
| EFILE_AGENCY_STATUS_CD | VARCHAR2(10)  | Null                 | The e-file status provided by the agency. For example: Accepted, Accepted with Warnings, Rejected.                              |
| COVERAGE_START_DT      | DATE          | Null                 | Date of the earliest report activity in the e-file.                                                                             |
| COVERAGE_END_DT        | DATE          | Null                 | Date of the latest report activity in the e-file.                                                                               |
| CORRECTION_FLG         | CHAR(1)       | Not Null             | Flag indicates if it is correction report.                                                                                      |
| OWNER_USER_ID          | VARCHAR2(60)  | Null                 | User who initially owns the report.                                                                                             |
| UI_DEF_FILE_NM         | VARCHAR2(100) | Null                 | User interface definition file name.                                                                                            |
| CREATE_USER_ID         | VARCHAR2(60)  | Null                 | The ID of the user that added the record.                                                                                       |
| CREATE_DTTM            | TIMESTAMP     | Null                 | The date and time when the record was added.                                                                                    |
| UPDATE_USER_ID         | VARCHAR2(60)  | Null                 | The ID of the user who updated the record.                                                                                      |
| VERSION_NO             | NUMBER(10)    | Not Null             | The date and time when the record was updated.                                                                                  |
| DELETE_FLG             | CHAR(1)       | Not Null             | A flag indicating whether the record is active.                                                                                 |

[Back to index](./index.md)
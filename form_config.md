# FORM_CONFIG

---

Form configuration table to link report and efile configuration

[Back to index](./index.md)

| Column Name               | Data Type     | Column Null Option   | Column Definition                                                                                                                                                                                        |
|:--------------------------|:--------------|:---------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| FORM_CONFIG_RK            | NUMBER(10)    | Not Null             | A sequential system generated key A surrogate key is added in the ETL process to ensure a unique identifier. May be used with validity date ranges in order to establish historical changes in the data. |
| FORM_AGENCY_CD            | VARCHAR2(32)  | Not Null             | A unique code to identify the government agency that published the form.                                                                                                                                 |
| FORM_TYPE_CD              | VARCHAR2(32)  | Not Null             | A unique code to identify the government form published by the agency defined in FORM_AGENCY_CD.                                                                                                         |
| FORM_COUNTRY_CD           | VARCHAR2(3)   | Null                 | A three character country code of the form.                                                                                                                                                              |
| EFFECTIVE_FROM_DTTM       | TIMESTAMP     | Not Null             | Start datetime when the form is effective to use. This field is for documentation purpose only. It is not used to determine if the form is effective.                                                    |
| EFFECTIVE_TO_DTTM         | TIMESTAMP     | Null                 | End datetime when the form is effective. Null in this column is used to indicate that the form is currently effective.                                                                                   |
| FORM_DESC                 | VARCHAR2(100) | Null                 | The description of the form.                                                                                                                                                                             |
| PREVIEW_MIME_TYPE_CD      | VARCHAR2(255) | Null                 | The standard mimetype of the preview report.                                                                                                                                                             |
| PREVIEW_FILE_PREFIX       | VARCHAR2(60)  | Null                 | The common prefix of all preview templates.                                                                                                                                                              |
| PREVIEW_DRIVER_PGM_NM     | VARCHAR2(60)  | Null                 | The SAS macro to be called by the ECMRR_PREVIEW stored process.                                                                                                                                          |
| PREVIEW_PREPROCESS_PGM_NM | VARCHAR2(60)  | Null                 | The SAS macro to be called by the preview driver program for transforming the RR data into form-ready data.                                                                                              |
| EFILE_FILE_PREFIX         | VARCHAR2(60)  | Null                 | The name of the output folder that will be used to store the output files.                                                                                                                               |
| EFILE_DRIVER_PGM_NM       | VARCHAR2(60)  | Null                 | The SAS macro to be called by the EFILE Driver stored process.                                                                                                                                           |
| EFILE_PREPROCESS_PGM_NM   | VARCHAR2(60)  | Null                 | The SAS macro to be called by the EFILE Driver program for transforming the RR data into e-file-ready data.                                                                                              |
| EFILE_MAX_RR_CNT          | NUMBER(6)     | Null                 | Indicates the maximum number of RR (reports) that can be included in an efile for that particular form.                                                                                                  |
| CREATE_USER_ID            | VARCHAR2(60)  | Null                 | The ID of the user that added the record.                                                                                                                                                                |
| CREATE_DTTM               | TIMESTAMP     | Null                 | The datetime when the record was added.                                                                                                                                                                  |
| UPDATE_USER_ID            | VARCHAR2(60)  | Null                 | The ID of the user who updated the record.                                                                                                                                                               |
| UPDATE_DTTM               | TIMESTAMP     | Null                 | The datetime when the record was updated.                                                                                                                                                                |
| DELETE_FLG                | CHAR(1)       | Not Null             | A flag indicating whether the record is active.                                                                                                                                                          |

[Back to index](./index.md)
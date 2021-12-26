# FORM_EFILE_RECORD_CONFIG

---

Controls the records of the output efile.

[Back to index](./index.md)

| Column Name              | Data Type      | Column Null Option   | Column Definition                                                                                                                                                                                        |
|:-------------------------|:---------------|:---------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| FORM_CONFIG_RK           | NUMBER(10)     | Not Null             | A sequential system generated key A surrogate key is added in the ETL process to ensure a unique identifier. May be used with validity date ranges in order to establish historical changes in the data. |
| FORM_EFILE_RECORD_SEQ_NO | NUMBER(10)     | Not Null             | The sequence number used to uniquely identify the record type of an e-file.                                                                                                                              |
| FORM_EFILE_RECORD_ID     | VARCHAR2(30)   | Not Null             | The ID used to uniquely identify the record type of an e-file.                                                                                                                                           |
| FORM_EFILE_RECORD_DESC   | VARCHAR2(1000) | Null                 | The description of the e-file record.                                                                                                                                                                    |
| RECORD_SORT_ORDER_NO     | NUMBER(10)     | Null                 | The order number in which the records will be placed into the e-file.                                                                                                                                    |
| RECORD_LENGTH_NO         | NUMBER(10)     | Null                 | The record length of the w-file.                                                                                                                                                                         |
| SOURCE_TABLE_NM          | VARCHAR2(30)   | Null                 | The name of the source table that will be used to populate the e-file record.                                                                                                                            |
| PAGE_BY_FIELD_NM         | VARCHAR2(30)   | Null                 | The name of the field for grouping the depending records together. For example, for FINCEN, the page types are BATCH, INSTITUTION, BRANCH and RR.                                                        |

[Back to index](./index.md)
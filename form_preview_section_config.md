# FORM_PREVIEW_SECTION_CONFIG

---

Controls the sections of the output efile.

[Back to index](./index.md)

| Column Name                 | Data Type      | Column Null Option   | Column Definition                                                                                                                                                                                        |
|:----------------------------|:---------------|:---------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| FORM_CONFIG_RK              | NUMBER(10)     | Not Null             | A sequential system generated key A surrogate key is added in the ETL process to ensure a unique identifier. May be used with validity date ranges in order to establish historical changes in the data. |
| FORM_PREVIEW_SECTION_SEQ_NO | NUMBER(10)     | Not Null             | The sequence number used to uniquely identify the form templates of a form.                                                                                                                              |
| FORM_PREVIEW_SECTION_ID     | VARCHAR2(32)   | Not Null             | The ID used to uniquely identify each form template.                                                                                                                                                     |
| SECTION_DESC                | VARCHAR2(1000) | Null                 | The description of the form template.                                                                                                                                                                    |
| SECTION_ORDER_NO            | NUMBER(10)     | Null                 | The order number in which the form templates will be placed into the final output.                                                                                                                       |
| SECTION_FILE_SUFFIX         | VARCHAR2(60)   | Null                 | The suffix of the file name for the form template.                                                                                                                                                       |
| SOURCE_TABLE_NM             | VARCHAR2(30)   | Null                 | The name of the source table used to populate the form template.                                                                                                                                         |

[Back to index](./index.md)
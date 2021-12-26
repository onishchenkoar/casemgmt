# FORM_PREVIEW_FIELD_CONFIG

---

Defines the mapping of the source data fields to the form fields.

[Back to index](./index.md)

| Column Name                 | Data Type      | Column Null Option   | Column Definition                                                                                                                                                                                        |
|:----------------------------|:---------------|:---------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| FORM_CONFIG_RK              | NUMBER(10)     | Not Null             | A sequential system generated key A surrogate key is added in the ETL process to ensure a unique identifier. May be used with validity date ranges in order to establish historical changes in the data. |
| FORM_PREVIEW_SECTION_SEQ_NO | NUMBER(10)     | Not Null             | The sequence number used to uniquely identify the form templates of a form.                                                                                                                              |
| FORM_PREVIEW_FIELD_SEQ_NO   | NUMBER(10,2)   | Not Null             | The sequence number used to uniquely identify the form fields in the form template.                                                                                                                      |
| SOURCE_FIELD_NM             | VARCHAR2(30)   | Null                 | The name of the source table field to be used for populating the form fields.                                                                                                                            |
| SOURCE_FIELD_NUM_FLG        | CHAR(1)        | Null                 | A flag that indicates if the source field or the result of the source field expression is numeric.                                                                                                       |
| SOURCE_FIELD_EXP            | VARCHAR2(4000) | Null                 | The expression used to transform the source field.                                                                                                                                                       |
| TARGET_FIELD_NM             | VARCHAR2(30)   | Not Null             | The name of the form field defined in the form template.                                                                                                                                                 |
| TARGET_FIELD_TYPE_CD        | VARCHAR2(10)   | Not Null             | The code for each type of form field. For example P1, P2, P3 and other depending on the number of parameters defined in the list.                                                                        |
| TARGET_FIELD_TYPE_PARM_LIST | VARCHAR2(1000) | Null                 | The list of '|' separated parameters to be passed to the macros.                                                                                                                                         |

[Back to index](./index.md)
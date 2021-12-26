# FORM_EFILE_FIELD_CONFIG

---

Defines the mapping of the source data fields to the target fields in EFILE.

[Back to index](./index.md)

| Column Name               | Data Type      | Column Null Option   | Column Definition                                                                                                                                                  |
|:--------------------------|:---------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| FORM_EFILE_RECORD_SEQ_NO  | NUMBER(10)     | Not Null             | The sequence number used to uniquely identify the record type of an e-flie.                                                                                        |
| FORM_EFILE_FIELD_SEQ_NO   | NUMBER(10)     | Not Null             | The sequence number used to uniquely identify the data fields of an e-file.                                                                                        |
| TARGET_FIELD_START_POS_NO | NUMBER(10)     | Null                 | The start position of the e-file field published by the government agency.                                                                                         |
| TARGET_FIELD_END_POS_NO   | NUMBER(10)     | Null                 | The end position of the e-file field published by the government agency.                                                                                           |
| TARGET_FIELD_NM           | VARCHAR2(100)  | Null                 | The name of the e-file field published by the government agency.                                                                                                   |
| TARGET_FIELD_LENGTH_NO    | NUMBER(10)     | Null                 | The length of the e-file field published by the government agency.                                                                                                 |
| TARGET_FIELD_DESC         | VARCHAR2(1000) | Null                 | The description of the e-file field published by the government agency.                                                                                            |
| SOURCE_FIELD_NM           | VARCHAR2(30)   | Null                 | The name of the field in the source table to be used for populating the form fields.                                                                               |
| SOURCE_FIELD_NUM_FLG      | CHAR(1)        | Null                 | A flag that indicates if the source field or the result of the source field expression is numeric.                                                                 |
| SOURCE_FIELD_EXP          | VARCHAR2(4000) | Null                 | The expression used to transform the source field.                                                                                                                 |
| SAS_FORMAT_NM             | VARCHAR2(40)   | Null                 | The name of the SAS format used to output the source field or the result of the source field expression. If the field is missing, the default format will be used. |

[Back to index](./index.md)
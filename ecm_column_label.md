# ECM_COLUMN_LABEL

---

Contains column label translation information.

[Back to index](./index.md)

| Column Name   | Data Type     | Column Null Option   | Column Definition                                                                                                                                                                                                                              |
|:--------------|:--------------|:---------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| TABLE_NM      | VARCHAR2(30)  | Not Null             | The name of the object or the name of the user-defined table that the column is associated with.                                                                                                                                               |
| COLUMN_NM     | VARCHAR2(30)  | Not Null             | The name of the column that the label is associated with.                                                                                                                                                                                      |
| LOCALE        | VARCHAR2(5)   | Not Null             | A locale supported by the application. The locale should follow the Java locale naming convention: a valid two-letter lowercase ISO 639 language code optionally appended with an underscore and a two-letter uppercase ISO 3166 country code. |
| LABEL_TXT     | VARCHAR2(100) | Not Null             | The translated label.                                                                                                                                                                                                                          |

[Back to index](./index.md)
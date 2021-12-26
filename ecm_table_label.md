# ECM_TABLE_LABEL

---

Contains table label translation information.

[Back to index](./index.md)

| Column Name   | Data Type     | Column Null Option   | Column Definition                                                                                                                                                                                                                              |
|:--------------|:--------------|:---------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| SOURCE_NM     | VARCHAR2(30)  | Not Null             | The source of the translation entry. Valid values are 'application' if the label translation comes from the standard application translation files or 'custom' if they come from one of the custom properties files.                           |
| OBJECT_NM     | VARCHAR2(30)  | Not Null             | The name of the object that the label is associated with. Valid values include 'CASE', 'INCIDENT', 'PARTY', 'FINANCIAL_ITEM' or '*' if the label applies to all objects.                                                                       |
| TABLE_NM      | VARCHAR2(30)  | Not Null             | The name of the table that the label is associated with.                                                                                                                                                                                       |
| LOCALE        | VARCHAR2(5)   | Not Null             | A locale supported by the application. The locale should follow the Java locale naming convention: a valid two-letter lowercase ISO 639 language code optionally appended with an underscore and a two-letter uppercase ISO 3166 country code. |
| LABEL_TXT     | VARCHAR2(100) | Not Null             | The translated label.                                                                                                                                                                                                                          |

[Back to index](./index.md)
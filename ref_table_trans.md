# REF_TABLE_TRANS

---

A record in the translation table corresponds to a single translation of a single entry in the REF_TABLE_VALUE table. The locale column should be to a Java-compliant locale-specifier.

[Back to index](./index.md)

| Column Name   | Data Type     | Column Null Option   | Column Definition                                                                                                                                                                                                                              |
|:--------------|:--------------|:---------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| REF_TABLE_NM  | VARCHAR2(30)  | Not Null             | Reference table name.                                                                                                                                                                                                                          |
| VALUE_CD      | VARCHAR2(32)  | Not Null             | Coded value.                                                                                                                                                                                                                                   |
| LOCALE        | VARCHAR2(5)   | Not Null             | A locale supported by the application. The locale should follow the Java locale naming convention: a valid two-letter lowercase ISO 639 language code optionally appended with an underscore and a two-letter uppercase ISO 3166 country code. |
| VALUE_DESC    | VARCHAR2(100) | Not Null             | The localized description for the given LOCALE of the reference table entry identified by the given REF_TABLE_NM and VALUE_CD.                                                                                                                 |

[Back to index](./index.md)
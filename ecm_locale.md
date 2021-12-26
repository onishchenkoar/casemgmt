# ECM_LOCALE

---

Contains localization data supported by the application.

[Back to index](./index.md)

| Column Name     | Data Type   | Column Null Option   | Column Definition                                                                                                                                                                                                                                                   |
|:----------------|:------------|:---------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| LOCALE          | VARCHAR2(5) | Not Null             | A locale supported by the application. The locale should follow the Java locale naming convention: a valid two-letter lowercase ISO 639 language code optionally appended with an underscore and a two-letter uppercase ISO 3166 country code.                      |
| FALLBACK_LOCALE | VARCHAR2(5) | Not Null             | The locale to consult next if there is no translation available for the locale specified by the LOCALE column. For example, if “en_GB” is a supported locale, it's fallback would be “en”. If the supported locale is “en”, then the fallback would be the default. |

[Back to index](./index.md)
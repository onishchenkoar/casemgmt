# INCIDENT_CONFIG

---

Defines the rules which determine the ui definition to display for a given incident, based on the incidnet's type, category and subcategory values. If a record includes null for category or subcategory, that is treated as a wildcard and that rule would apply for any value in that column. In situations where multiple rules apply, the sequence number is treated as the priority; the matching rule with the smallest sequence number will be selected.

[Back to index](./index.md)

| Column Name             | Data Type     | Column Null Option   | Column Definition                                                                                                                                                                                                                          |
|:------------------------|:--------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| INCIDENT_CONFIG_SEQ_NO  | NUMBER(10)    | Not Null             | Incident configuration sequence number. The sequence number is also used as a priority when multiple configurations apply for a given incident. If multiple configurations apply, the one with the smaller sequence number will be chosen. |
| INCIDENT_TYPE_CD        | VARCHAR2(32)  | Not Null             | Incident type code.                                                                                                                                                                                                                        |
| INCIDENT_CATEGORY_CD    | VARCHAR2(32)  | Null                 | Incident category code.                                                                                                                                                                                                                    |
| INCIDENT_SUBCATEGORY_CD | VARCHAR2(32)  | Null                 | Incident subcategory code.                                                                                                                                                                                                                 |
| UI_DEF_FILE_NM          | VARCHAR2(100) | Not Null             | User interface definition file name.                                                                                                                                                                                                       |

[Back to index](./index.md)
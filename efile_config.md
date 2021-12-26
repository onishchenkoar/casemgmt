# EFILE_CONFIG

---

DefineDefines the rules which determine the ui definition to display for a given efile, based on the efile's type, category and subcategory values. If a record includes null for category or subcategory, that is treated as a wildcard and that rule would apply for any value in that column. In situations where multiple rules apply, the sequence number is treated as the priority; the matching rule with the smallest sequence number will be selected.

[Back to index](./index.md)

| Column Name   | Data Type    | Column Null Option   | Column Definition                                                                            |
|:--------------|:-------------|:---------------------|:---------------------------------------------------------------------------------------------|
| FORM_TYPE_CD  | VARCHAR2(32) | Not Null             | Unique code to define the government form published by the agency defined in FORM_AGENCY_CD. |

[Back to index](./index.md)
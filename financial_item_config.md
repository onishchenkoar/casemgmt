# FINANCIAL_ITEM_CONFIG

---

The financial_item config table maps which ui definition to use for each financial_item type. The financial_item_config tablediffers from the other config tables. Financial items are configured solely on the financial_item type code. Case, Incident and Party are configured based on type, category and sub-category.

[Back to index](./index.md)

| Column Name                  | Data Type     | Column Null Option   | Column Definition                                                                                                                                                                                             |
|:-----------------------------|:--------------|:---------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| FINANCIAL_ITEM_CONFIG_SEQ_NO | NUMBER(10)    | Not Null             | The primary key for the FINANCIAL_ITEM_CONFIG table.                                                                                                                                                          |
| FINANCIAL_ITEM_TYPE_CD       | VARCHAR2(32)  | Not Null             | The financial item type being configured. This value should reference an entry in the financial item type reference table (stored in the REF_TABLE_VALUE table with REF_TABLE_NM = 'RT_FINANCIAL_ITEM_TYPE'). |
| UI_DEF_FILE_NM               | VARCHAR2(100) | Not Null             | The UI definition file to use for financial items of the given financial item type.                                                                                                                           |

[Back to index](./index.md)
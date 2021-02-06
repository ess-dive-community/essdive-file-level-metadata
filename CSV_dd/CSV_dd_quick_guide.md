# Quick guide for the CSV Data Dictionary (CSV_dd)

Elements of the data dictionary:  
* [Column_name](#column-name)  
* [Unit](#unit)  
* [Definition](#definition)  
* [Column_long_name](#column-long-name)  
* [Data_type](#data-type)  


---  

### Column name  
|Metadata_Element|Column_Name|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting format statement|Column name from the data file.|
|Reporting format definition|Provide entries for each Column Name from the data matrix in the data file.|
|Required, Recommended or Optional|required|

### Unit  
|Metadata_Element|Unit|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting format statement|Provide the format or variable unit of measurement.|
|Reporting format definition|Provide variable units of measurement. Insert "N/A" when units aren't applicable. Data should be represented with units of measurement approved by the International System of Units (SI). Non-SI units are accepted for use and should be defined and referenced.|
|Required, Recommended or Optional|required|

### Definition
|Metadata_Element|Definition|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting format statement|A complete unambiguous description.|
|Reporting format definition|A complete unambiguous description. Information may include: formulas used to calculate entry; definitions of coding systems (e.g. missing values, quality flags, etc.); detection limits; timestamp calculation; measurement of uncertainty, etc.|
|Required, Recommended or Optional|required|

### Column long name  
|Metadata_Element|Column_Long_Name|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting format statement|Human-readable name.|
|Reporting format definition|Longer human-readable column name. Sometimes this may be identical to Definition or even column_name.|
|Required, Recommended or Optional|recommended|

### Data type
|Metadata_Element|Data_Type|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting format statement|Define the data type.|
|Reporting format definition|Define the data type for each column (e.g. text, numeric, date)|
|Required, Recommended or Optional|recommended|

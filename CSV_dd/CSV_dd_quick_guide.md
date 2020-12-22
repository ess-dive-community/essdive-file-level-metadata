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
|Standard Statement|Column name from the data file.|
|Standard Definition|Provide entries for each Column Name from the data matrix in the data file.|
|Required, Recommended or Optional|required|

### Unit  
|Metadata_Element|Unit|
|:----------------------------------------------------|:----------------------------------------------------|
|Standard Statement|Provide the format or variable unit of measurement.|
|Standard Definition|Provide variable units of measurement. Insert "N/A" when units aren't applicable. Data should be represented with units of measurement approved by the International System of Units (SI). Non-SI units are accepted for use and should be defined and referenced.|
|Required, Recommended or Optional|required|

### Definition
|Metadata_Element|Definition|
|:----------------------------------------------------|:----------------------------------------------------|
|Standard Statement|A complete unambiguous description.|
|Standard Definition|A complete unambiguous description. Information may include: formulas used to calculate entry; definitions of coding systems (e.g. missing values, quality flags, etc.); detection limits; timestamp calculation; measurement of uncertainty, etc.|
|Required, Recommended or Optional|required|

### Column long name  
|Metadata_Element|Column_Long_Name|
|:----------------------------------------------------|:----------------------------------------------------|
|Standard Statement|Human-readable name.|
|Standard Definition|Longer human-readable column name. Sometimes this may be identical to Definition or even column_name.|
|Required, Recommended or Optional|recommended|

### Data type
|Metadata_Element|Data_Type|
|:----------------------------------------------------|:----------------------------------------------------|
|Standard Statement|Define the data type.|
|Standard Definition|Define the data type for each column (e.g. text, numeric, date)|
|Required, Recommended or Optional|recommended|
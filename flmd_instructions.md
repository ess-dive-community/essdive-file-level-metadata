# ESS-DIVE File-level Metadata Reporting Format Instructions

1. Create file-level metadata for each data file using the template.  
&nbsp;&nbsp;&nbsp;&nbsp;a. Start new row for each data file    
&nbsp;&nbsp;&nbsp;&nbsp;b. Use "\*" wildcard when the FLMD applies to multiple files.   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i. For example - the same FLMD applies to all soil core files in this data package - "soil_cores_*.csv"

2. Follow the instructions in the [FLMD quick guide](flmd_quick_guide.md).
3. Use the [FLMD template](flmd_template.xlsx).
4. Save the FLMD template following the CSV Reporting Format guidance.
5. For CSV data files, create a [CSV Data Dictionary](/CSV_dd/CSV_dd_instructions.md) to describe the fields and other attributes of your CSV data file

**Notes**

* Fields common to ESS-DIVE Package Level Metadata are consistent in format structure.  

**Contents of the Elements**  

* File_Name  
* File_Description  
* Standard  
* UTC_Offset  
* File_Version  
* Contact  
* Start_Date  
* End_Date  
* Northwest_Latitude_Coordinate  
* Northwest_Longitude_Coordinate  
* Southeast_Latitude_Coordinate  
* Southeast_Longitude_Coordinate  
* Latitude  
* Longitude  
* Missing_Value_Codes  
* Notes  
* Field_Name_Orientation  


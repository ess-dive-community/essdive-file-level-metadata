# Instructions

## ESS-DIVE File-level Metadata Reporting Format

## Instructions

1. Create file-level metadata for each data package using the template  
&nbsp;&nbsp;&nbsp;a. Start new row for each file and include all files  
&nbsp;&nbsp;&nbsp;b. Use "\*" wildcard when the FLMD applies to multiple files  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i. For example - the same FLMD applies to all soil core files in this data package - "soil_cores_\*\.csv"  
2. Follow the instructions in the [FLMD quick guide](documents/flmd_quick_guide.md)  
3. Use the [FLMD template](https://github.com/ess-dive-community/essdive-file-level-metadata/tree/3acd84067cf980484b4b86e95dbdcace42db3796/flmd_template.xlsx)  
4. Save the FLMD template following the CSV Reporting Format guidance. We recommend naming the flmd file "flmd.csv" or you can include a prefix in the form of "\*\_flmd.csv"  
5. For CSV data files, create a [CSV Data Dictionary](csv_dd_instructions/) to describe the fields and other attributes of your CSV data file 
6. For zip files, recommend including the FLMD outside the zip file but may also include it in the zip file  

**Notes**

* Fields common to ESS-DIVE Package Level Metadata are consistent in format structure.  

**Contents of the Elements**

* File\_Name  
* File\_Description  
* Standard  
* UTC\_Offset  
* File\_Version  
* Contact  
* Start\_Date  
* End\_Date  
* Northwest\_Latitude\_Coordinate  
* Northwest\_Longitude\_Coordinate  
* Southeast\_Latitude\_Coordinate  
* Southeast\_Longitude\_Coordinate  
* Latitude  
* Longitude  
* Missing\_Value\_Codes  
* Notes  
* Field\_Name\_Orientation  


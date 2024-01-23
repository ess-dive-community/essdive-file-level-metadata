# Instructions for ESS-DIVE File Level Metadata Reporting Format

1. Create file-level metadata for each data set using the provided template  
&nbsp;&nbsp;&nbsp;a. Start new row for each file and include all files  
&nbsp;&nbsp;&nbsp;b. Use "\*" wildcard when an FLMD entry applies to multiple files with similar naming conventions
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i. For example - the same FLMD row information applies to all soil core files in this data package - "soil\_cores\_\*\.csv"  
2. Follow the instructions in the [FLMD quick guide](flmd_quick_guide.md)  
3. Use the [FLMD template](https://github.com/ess-dive-community/essdive-file-level-metadata/blob/master/flmd_template.xlsx)  
4. Save the FLMD template as a CSV. Name the flmd file "flmd.csv" or you can include a prefix in the form of "\*\_flmd.csv"  
5. For CSV data files, create a [CSV Data Dictionary](CSV_dd/) to describe the fields and other attributes of your CSV data file. The data dictionary file should be listed in your FLMD file (described in step 1) 
6. We recommend including the FLMD outside of any zip files for easy identification, but you may also include it in the zip file
7. If submitting your dataset to ESS-DIVE, include the keyword **ESS-DIVE File Level Metadata Reporting Format** in the package-level metadata.

**Notes**

* Fields common to ESS-DIVE Package Level Metadata are consistent in format structure  

**Contents of the Elements**

* file_name 
* file_description
* standard  
* utc_offset 
* file_version
* contact  
* date_start 
* date_end
* missing_value_codes
* data_orientation  
* header_row
* column_or_row_name_position
* northwest_latitude_coordinate
* northwest_longitude_coordinate 
* southeast_latitude_coordinate 
* southeast_longitude_coordinate
* latitude  
* longitude  
* notes


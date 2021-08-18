# CSV Data Dictionary

## Instructions

1. Create a CSV data dictionary using the [CSV\_dd\_template](https://github.com/ess-dive-community/essdive-file-level-metadata/blob/master/CSV_dd/CSV_dd_template.csv).  You can create either: 
 
        a. One data dictionary for each data file or  

        b. One data dictionary representing all data files in your dataset    

2. See the [CSV\_dd\_quick\_guide](csv_dd_quick_guide.md) for more details about completing the template  
3. Enter a new row in the data dictionary for each column/row name in your data matrix 
   
        a. Use "\*" wildcard when the description applies to multiple column/row names  
        
        b. For example - if the same description applies to all spectra data column names in the data file(s)   
        
            i. one row in the data dictionary can refer to "wave_\*\" and this definition will be understood to apply to multiple column names within a data sheet     
            
4. View an example [CSV\_dd\_example](csv_dd_example.md)  

5. Save the CSV\_dd template following the [CSV Reporting Format guidance](https://github.com/ess-dive-community/essdive-csv-structure) with the filename "dd.csv" or "\*\_dd.csv". Alternatively you may choose to name you data dictionary: 
   
    a. With the same name as the associated data file, but include '\_dd.csv' at the end of the file name  
    b. Create a unique filename for your data dictionary  
    c. Incorporate a wildcard into the filename if data dictionary applies to multiple data files (for example - "soil_cores_\*\_dd.csv")  

**Contents of the CSV\_dd**

For each variable provide the following:

* Column or Row Name  
* Unit  
* Definition  
* Column or Row Long Name    
* Data Type  

**Notes**  

Following the recommended format and structure of the CSV Reporting Format will facilitate File-level Metadata extraction of some fields using the [File Level Metadata Extractor](https://code.ornl.gov/ngee-arctic/ess-dive-meta)


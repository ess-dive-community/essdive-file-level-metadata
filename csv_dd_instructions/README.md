# CSV Data Dictionary

## Instructions

1. Create a CSV data dictionary using the [CSV\_dd\_template](https://github.com/ess-dive-community/essdive-file-level-metadata/blob/master/CSV_dd/CSV_dd_template.csv) 
 
        a. Create a data dictionary for each data file or  

        b. Create one data dictionary representing all data files.    

3. See the [CSV\_dd\_quick\_guide](csv_dd_quick_guide.md) for more details about completing the template  
4. Enter a new row for each field in the data matrix.

        a. Use "\*" wildcard when the description applies to multiple fields.  

        b. For example - the same description applies to all spectra data fields in the data file(s)   

            i. "wave_\*\"   
6. View an example [CSV\_dd\_example](csv_dd_example.md).  
7. Save the CSV\_dd template following the [CSV Reporting Format guidance](https://github.com/ess-dive-community/essdive-csv-structure) with the filename "dd.csv" or "\*\_dd.csv"  

        a. CSV_dd could have the same name as the associated data filename  

        b. Unique filename
        
        c. Wildcard filename if CSV_dd applies to multiple data files (for example - "soil_cores_\*\_dd.csv")      


**Contents of the CSV\_dd**

For each variable provide the following:

* Field name  
* Unit  
* Definition  
* Field long name  
* Data type  

**Notes**

Following the recommended format and structure of the CSV Reporting Format will facilitate FLMD extraction of some fields using the [File Level Metadata Extractor](https://code.ornl.gov/ngee-arctic/ess-dive-meta)


# CSV Data Dictionary

## Instructions

1. Create a CSV data dictionary using the [CSV\_dd\_template](https://github.com/ess-dive-community/essdive-file-level-metadata/blob/master/CSV_dd/CSV_dd_template.csv)  
2. See the [CSV\_dd\_quick\_guide](csv_dd_quick_guide.md) for more details about completing the template  
3. Enter a new row for each column in the data matrix.  
4. View an example [CSV\_dd\_example](csv_dd_example.md).  
5. Save the CSV\_dd template following the [CSV Reporting Format guidance](https://github.com/ess-dive-community/essdive-csv-structure).  
6. Recommend naming the CSV\_dd with same name as the original data filename and append "\_dd".  

        a. Use "\*" wildcard when the CSV\_dd applies to multiple CSV data files.  

        b. For example - the same CSV\_dd applies to all soil core files in this data package   

            i. "soil_cores_\*\_dd.csv"  

**Contents of the CSV\_dd**

For each variable provide the following:

* Column name  
* Unit  
* Definition  
* Column long name  
* Data type  

**Notes**

Following the recommended format and structure of the CSV Reporting Format will facilitate FLMD extraction of some fields using the [File Level Metadata Extractor](https://code.ornl.gov/ngee-arctic/ess-dive-meta)


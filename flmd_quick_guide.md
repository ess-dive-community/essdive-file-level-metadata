# Quick guide for ESS-DIVE File-level Metadata Reporting Format

Elements of the reporting format:  
* [file_name](#file-name)  
* [file_description](#file-description)  
* [standard](#standard)  
* [utc_offset](#utc-offset)  
* [file_version](#file-version)  
* [contact](#contact)  
* [date_start](#date-start)  
* [date_end](#date-end)
* [missing_value_codes](#missing-value-codes)  
* [data_orientation](#data-orientation)
* [header_rows](#header-rows)
* [column_or_row_name_position](#column-or-row-name-position)
* [northwest_latitude_coordinate](#northwest-latitude-coordinate)  
* [northwest_longitude_coordinate](#northwest-longitude-coordinate)  
* [southeast_latitude_coordinate](#southeast-latitude-coordinate)  
* [southeast_longitude_coordinate](#southeast-longitude-coordinate)  
* [latitude](#latitude)  
* [longitude](#longitude)  
* [notes](#notes)  
 

---  

### File Name  
|Metadata Element|file_name|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Name of the file|
|Reporting Format Definition|Provide the name of the associated file. File names should be unique and be as descriptive as possible about the file contents. Use only letters (e.g. CamelCase), numbers, and underscores. Do not include spaces. Hyphens allowed but not preferred. Use "\*" wildcard when the FLMD applies to multiple files. For example - the same FLMD applies to all soil core files in this data package - "soil&#95;cores&#95;\*\.csv"|
|Required, Recommended or Optional|required|
|Format||

### File Description
|Metadata Element|file_description|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|A brief description of the file|
|Reporting Format Definition|A brief description (minimum 30 characters) of the file and what distinguishes this file from other files in the data package. Include information about the type of data (images, observations, experimental, etc.) |
|Required, Recommended or Optional|required|
|Format||

### Standard  
|Metadata Element|standard|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|standard applied to the data file.|
|Reporting Format Definition|Identify if an ESS-DIVE Reporting Format or any other data or metadata standard was applied to the data file. Standard names for the ESS-DIVE reporting formats are available in the Standard FLMD Term List.|
|Required, Recommended or Optional|strongly recommended|
|Format||

### UTC Offset  
|Metadata Element|utc_offset|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Local Standard Time Offset|
|Reporting Format Definition|Report the Local Standard Time offset (+/- #hours) or time zone (abbreviations allowed). Do not report time using Daylight Savings Time.|
|Required, Recommended or Optional|strongly recommended|
|Format||

### File Version  
|Metadata Element|file_version|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|The version of the file.|
|Reporting Format Definition|This is the version of the data file being described in the FLMD. The data file version is assigned by the data provider and not by the system. This would change if the data file is updated after the data package is published. Changes should be explained in the Notes field.|
|Required, Recommended or Optional|optional|
|Format||

### Contact  
|Metadata Element|contact|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Contact for the file.|
|Reporting Format Definition|Provide first and last name of the contact for the file. This should be someone with information already recorded at the Data Package Level. If you would like to include multiple contacts, separate them using a semi-colon.|
|Required, Recommended or Optional|optional|
|Format|text|

### Date Start  
|Metadata Element|date_start|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|The earliest date in the file.|
|Reporting Format Definition|All dates must follow the ISO 8601 standard. This field can be date only following the ISO 8601 standard (YYYY-MM-DD) and completed to known precision (e.g. YYYY-MM, YYYY). The FLMD Extractor can extract the start/end date from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format|yyyy-mm-dd|

### Date End
|Metadata Element|date_end|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|The latest date in the file.|
|Reporting Format Definition|All dates must follow the ISO 8601 standard. This field can be date only following the ISO 8601 standard (YYYY-MM-DD) and completed to known precision (e.g. YYYY-MM, YYYY).|
|Required, Recommended or Optional|optional|
|Format|yyyy-mm-dd|

### Missing Value Codes
|Metadata Element|missing_value_codes|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Report missing value codes|
|Reporting Format Definition|Report all Missing Value Codes. For columns containing numeric data, use "-9999" as the missing value code (or modify to match significant figures given the data). For columns containing character data, use "N/A" as the missing value code. If entering more than one missing value code, use a vertical bar "\|" or semicolon ";" instead of a comma or protect the comma with matching double quotation marks around the entire value. For more information about commas not meant to be a delimiter (e.g. used within a cell), refer to the Delimiter section of the CSV Reporting Format Detailed Guide.|
|Required, Recommended or Optional|optional|
|Format||

### Data Orientation  
|Metadata Element|data_orientation|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Orientation of tabular data|
|Reporting Format Definition|Describe how the data are organized within the data matrix. Choose between "horizontal" (i.e., data are organized in rows) or "vertical" (i.e., data are organized in columns).|
|Required, Recommended or Optional|optional|
|Format||  

### Header Rows
|Metadata Element|header_rows|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Number of header rows.|
|Reporting Format Definition|Provide the number of header rows that occur _after_ the column or row names in a file and _before_ the data begins. This field is marked as optional, but is required if the dataset has multiple header rows.|
|Required, Recommended or Optional|optional|
|Format|number|

### Column or Row Name Position
|Metadata Element|column_or_row_name_position|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Position of the column or row that contains the column or row names.|
|Reporting Format Definition|Provide the row or column number that contains the header names. This field is not required if there are no rows (if data is horizontally oriented) or columns (if data are vertically oriented) before the row/column names. If not included, it will be assumed that header names are in row 0 (vertically oriented) or column 0 (horizontally oriented). If there are rows/columns after the header names, note these using the header_rows field.|
|Required, Recommended or Optional|optional|
|Format|number|

### Northwest Latitude Coordinate
|Metadata Element|northwest_latitude_coordinate|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Northwest latitude Coordinate for non-point location.|
|Reporting Format Definition|This is part of a coordinate pair to form the Northwest corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format|decimal degrees|

### Northwest Longitude Coordinate
|Metadata Element|northwest_longitude_coordinate|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Northwest Longitude Coordinate for non-point location.|
|Reporting Format Definition|This is part of a coordinate pair to form the Northwest corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format|decimal degrees|

### Southeast Latitude Coordinate
|Metadata Element|southeast_latitude_coordinate|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Southeast Latitude Coordinate for non-point location.|
|Reporting Format Definition|This is part of a coordinate pair to form the Southeast corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format|decimal degrees|

### Southeast Longitude Coordinate
|Metadata Element|southeast_longitude_coordinate|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Southeast Longitude Coordinate for non-point location.|
|Reporting Format Definition|This is part of a coordinate pair to form the Southeast corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format|decimal degrees|

### Latitude  
|Metadata Element|latitude|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Coordinate for single point location.|
|Reporting Format Definition|This field is paired with "Longitude" to create a coordinate pair for a single point. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format||

### Longitude  
|Metadata Element|longitude|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Coordinate for single point location.|
|Reporting Format Definition|This field is paired with "Latitude" to create a coordinate pair for a single point. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format||

### Notes  
|Metadata Element|notes|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Any information the provider would like to add.|
|Reporting Format Definition|Information provided would be data file specific. Details may include details on data file versioning, reporting format, software requirements, data quality, etc.|
|Required, Recommended or Optional|optional|
|Format||

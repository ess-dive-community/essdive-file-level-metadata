# Quick guide for ESS-DIVE File-level Metadata Reporting Format

Elements of the reporting format:  
* [File_Name](#file-name)  
* [File_Description](#file-description)  
* [Standard](#standard)  
* [UTC_Offset](#utc-offset)  
* [File_Version](#file-version)  
* [Contact](#contact)  
* [Date_Start](#date-start)  
* [Date_End](#date-end)  
* [Northwest_Latitude_Coordinate](#northwest-latitude-coordinate)  
* [Northwest_Longitude_Coordinate](#northwest-longitude-coordinate)  
* [Southeast_Latitude_Coordinate](#southeast-latitude-coordinate)  
* [Southeast_Longitude_Coordinate](#southeast-longitude-coordinate)  
* [Latitude](#latitude)  
* [Longitude](#longitude)  
* [Missing_Value_Codes](#missing-value-codes)  
* [Data_Orientation](#data-orientation)  
* [Notes](#notes)  
 

---  

### File Name  
|Metadata Element|File_Name|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Name of the file|
|Reporting Format Definition|Provide the name of the associated file. File names should be unique and be as descriptive as possible about the file contents. Use only letters (e.g. CamelCase), numbers, and underscores. Do not include spaces. Hyphens allowed but not preferred. Use "\*" wildcard when the FLMD applies to multiple files. For example - the same FLMD applies to all soil core files in this data package - "soil&#95;cores&#95;\*\.csv"|
|Required, Recommended or Optional|required|
|Format||

### File Description
|Metadata Element|File_Description|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|A brief description of the file|
|Reporting Format Definition|A brief description (minimum 30 characters) of the file and what distinguishes this file from other files in the data package. Include information about the type of data (images, observations, experimental, etc.) |
|Required, Recommended or Optional|required|
|Format||

### Standard  
|Metadata Element|Standard|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Standard applied to the data file.|
|Reporting Format Definition|Identify if an ESS-DIVE Reporting Format or any other data or metadata standard was applied to the data file.|
|Required, Recommended or Optional|strongly recommended|
|Format||

### UTC Offset  
|Metadata Element|UTC_Offset|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Local Standard Time Offset|
|Reporting Format Definition|Report the Local Standard Time offset (+/- #hours) or time zone (abbreviations allowed). Do not report time using Daylight Savings Time.|
|Required, Recommended or Optional|strongly recommended|
|Format||

### File Version  
|Metadata Element|File_Version|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|The version of the file.|
|Reporting Format Definition|This is the version of the data file being described in the FLMD. The data file version is assigned by the data provider and not by the system. This would change if the data file is updated after the data package is published. Changes should be explained in the Notes field.|
|Required, Recommended or Optional|optional|
|Format||

### Contact  
|Metadata Element|Contact|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Contact for the file.|
|Reporting Format Definition|Provide first and last name of the contact for the file. This should be someone with information already recorded at the Data Package Level.|
|Required, Recommended or Optional|optional|
|Format||

### Date Start  
|Metadata Element|Date_Start|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|The earliest date in the file.|
|Reporting Format Definition|All dates must follow the ISO 8601 standard. This field can be date only following the ISO 8601 standard (YYYY-MM-DD) and completed to known precision (e.g. YYYY-MM, YYYY). The FLMD Extractor can extract the start/end date from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format|yyyy-mm-dd|

### Date End
|Metadata Element|Date_End|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|The latest date in the file.|
|Reporting Format Definition|All dates must follow the ISO 8601 standard. This field can be date only following the ISO 8601 standard (YYYY-MM-DD) and completed to known precision (e.g. YYYY-MM, YYYY). The FLMD Extractor can extract the start/end date from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format|yyyy-mm-dd|

### Northwest Latitude Coordinate
|Metadata Element|Northwest_Latitude_Coordinate|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Northwest Latitude Coordinate for non-point location.|
|Reporting Format Definition|This is part of a coordinate pair to form the Northwest corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format|decimal degrees|

### Northwest Longitude Coordinate
|Metadata Element|Northwest_Longitude_Coordinate|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Northwest Longitude Coordinate for non-point location.|
|Reporting Format Definition|This is part of a coordinate pair to form the Northwest corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format|decimal degrees|

### Southeast Latitude Coordinate
|Metadata Element|Southeast_Latitude_Coordinate|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Southeast Latitude Coordinate for non-point location.|
|Reporting Format Definition|This is part of a coordinate pair to form the Southeast corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format|decimal degrees|

### Southeast Longitude Coordinate
|Metadata Element|Southeast_Longitude_Coordinate|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Southeast Longitude Coordinate for non-point location.|
|Reporting Format Definition|This is part of a coordinate pair to form the Southeast corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format|decimal degrees|

### Latitude  
|Metadata Element|Latitude|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Coordinate for single point location.|
|Reporting Format Definition|This field is paired with "Longitude" to create a coordinate pair for a single point. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format||

### Longitude  
|Metadata Element|Longitude|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Coordinate for single point location.|
|Reporting Format Definition|This field is paired with "Latitude" to create a coordinate pair for a single point. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.|
|Required, Recommended or Optional|optional|
|Format||

### Missing Value Codes
|Metadata Element|Missing_Value_Codes|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Report missing value codes|
|Reporting Format Definition|Report all Missing Value Codes. For columns containing numeric data, use "-9999" as the missing value code (or modify to match significant figures given the data). For columns containing character data, use "N/A" as the missing value code. If entering more than one missing value code, use a vertical bar "\|" or semicolon ";" instead of a comma or protect the comma with matching double quotation marks around the entire value. For more information about commas not meant to be a delimiter (e.g. used within a cell), refer to the Delimiter section of the CSV Reporting Format Detailed Guide.|
|Required, Recommended or Optional|optional|
|Format||

### Data Orientation  
|Metadata Element|Data_Orientation|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Orientation of tabular data|
|Reporting Format Definition|Describe how the data are organized within the data matrix. Choose between "horizontal" (i.e., data are organized in rows) or "vertical" (i.e., data are organized in columns).|
|Required, Recommended or Optional|optional|
|Format||  

### Notes  
|Metadata Element|Notes|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Any information the provider would like to add.|
|Reporting Format Definition|Information provided would be data file specific. Details may include details on data file versioning, reporting format, software requirements, data quality, etc.|
|Required, Recommended or Optional|optional|
|Format||

# FLMD quick guide

Elements of the reporting format:

* [File\_Name](flmd_quick_guide.md#file-name)  
* [File\_Description](flmd_quick_guide.md#file-description)  
* [Standard](flmd_quick_guide.md#standard)  
* [UTC\_Offset](flmd_quick_guide.md#utc-offset)  
* [File\_Version](flmd_quick_guide.md#file-version)  
* [Contact](flmd_quick_guide.md#contact)  
* [Start\_Date](flmd_quick_guide.md#start-date)  
* [End\_Date](flmd_quick_guide.md#end-date)  
* [Northwest\_Latitude\_Coordinate](flmd_quick_guide.md#northwest-latitude-coordinate)  
* [Northwest\_Longitude\_Coordinate](flmd_quick_guide.md#northwest-longitude-coordinate)  
* [Southeast\_Latitude\_Coordinate](flmd_quick_guide.md#southeast-latitude-coordinate)  
* [Southeast\_Longitude\_Coordinate](flmd_quick_guide.md#southeast-longitude-coordinate)  
* [Latitude](flmd_quick_guide.md#latitude)  
* [Longitude](flmd_quick_guide.md#longitude)  
* [Missing\_Value\_Codes](flmd_quick_guide.md#missing-value-codes)  
* [Notes](flmd_quick_guide.md#notes)  
* [Field\_Name\_Orientation](flmd_quick_guide.md#field-name-orientation)  

## File name

| Metadata Element | File\_Name |
| :--- | :--- |
| Reporting Format Statement | Name of the file |
| Reporting Format Definition | Provide the name of the associated file. Filenames should be unique and be as descriptive as possible about the file contents. Use only letters \(e.g. CamelCase\), numbers, and underscores "\_". Do not include spaces. Hyphens allowed but not preferred. Use "\*" wildcard when the FLMD applies to multiple files. For example - the same FLMD applies to all soil core files in this data package - "soil\_cores_\*.csv" |
| Required, Recommended or Optional | required |
| Format |  |

## File description

| Metadata Element | File\_Description |
| :--- | :--- |
| Reporting Format Statement | A brief description of the file |
| Reporting Format Definition | A brief description \(minimum 30 characters\) of the file and what distinguishes this file from other files in the data package. Include information about the type of data \(images, observations, experimental, etc.\) |
| Required, Recommended or Optional | required |
| Format |  |

## Standard

| Metadata Element | Standard |
| :--- | :--- |
| Reporting Format Statement | Standard applied to the data file. |
| Reporting Format Definition | Identify if an ESS-DIVE Reporting Format or any other standard was applied to the data file. |
| Required, Recommended or Optional | strongly recommended |
| Format |  |

## UTC Offset

| Metadata Element | UTC\_Offset |
| :--- | :--- |
| Reporting Format Statement | Local Standard Time Offset |
| Reporting Format Definition | Report the Local Standard Time offset \(+/- \#hours\) or time zone \(abbreviations allowed\). Do not report time using Daylight Savings Time. |
| Required, Recommended or Optional | strongly recommended |
| Format |  |

## File version

| Metadata Element | File\_Version |
| :--- | :--- |
| Reporting Format Statement | The version of the file. |
| Reporting Format Definition | This is the version of the data file being described in the FLMD. The data file version is assigned by the data provider and not by the system. This would change if the data file is updated after the data package is published. Changes should be explained in the Notes field. |
| Required, Recommended or Optional | optional |
| Format |  |

## Contact

| Metadata Element | Contact |
| :--- | :--- |
| Reporting Format Statement | Contact for the file. |
| Reporting Format Definition | Contact for the file. This should be someone with information already recorded at the Data Package Level. |
| Required, Recommended or Optional | optional |
| Format |  |

## Start date

| Metadata Element | Start\_Date |
| :--- | :--- |
| Reporting Format Statement | The earliest date in the file. |
| Reporting Format Definition | All dates must follow the ISO 8601 standard. This field can be date only following the ISO 8601 standard \(YYYY-MM-DD\) and completed to known precision \(e.g. YYYY-MM, YYYY\). The FLMD Extractor can extract the start/end date from a CSV file following the CSV Reporting Format. |
| Required, Recommended or Optional | optional |
| Format | yyyy-mm-dd |

## End date

| Metadata Element | End\_Date |
| :--- | :--- |
| Reporting Format Statement | The latest date in the file. |
| Reporting Format Definition | All dates must follow the ISO 8601 standard. This field can be date only following the ISO 8601 standard \(YYYY-MM-DD\) and completed to known precision \(e.g. YYYY-MM, YYYY\). The FLMD Extractor can extract the start/end date from a CSV file following the CSV Reporting Format. |
| Required, Recommended or Optional | optional |
| Format | yyyy-mm-dd |

## Northwest latitude coordinate

| Metadata Element | Northwest\_Latitude\_Coordinate |
| :--- | :--- |
| Reporting Format Statement | Northwest Latitude Coordinate for non-point location. |
| Reporting Format Definition | This is part of a coordinate pair to form the Northwest corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format. |
| Required, Recommended or Optional | optional |
| Format | decimal degrees |

## Northwest longitude coordinate

| Metadata Element | Northwest\_Longitude\_Coordinate |
| :--- | :--- |
| Reporting Format Statement | Northwest Longitude Coordinate for non-point location. |
| Reporting Format Definition | This is part of a coordinate pair to form the Northwest corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format. |
| Required, Recommended or Optional | optional |
| Format | decimal degrees |

## Southeast latitude coordinate

| Metadata Element | Southeast\_Latitude\_Coordinate |
| :--- | :--- |
| Reporting Format Statement | Southeast Latitude Coordinate for non-point location. |
| Reporting Format Definition | This is part of a coordinate pair to form the Southeast corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format. |
| Required, Recommended or Optional | optional |
| Format | decimal degrees |

## Southeast longitude coordinate

| Metadata Element | Southeast\_Longitude\_Coordinate |
| :--- | :--- |
| Reporting Format Statement | Southeast Longitude Coordinate for non-point location. |
| Reporting Format Definition | This is part of a coordinate pair to form the Southeast corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format. |
| Required, Recommended or Optional | optional |
| Format | decimal degrees |

## Latitude

| Metadata Element | Latitude |
| :--- | :--- |
| Reporting Format Statement | Coordinate for single point location. |
| Reporting Format Definition | This field is paired with "Longitude" to create a coordinate pair for a single point. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format. |
| Required, Recommended or Optional | optional |
| Format |  |

## Longitude

| Metadata Element | Longitude |
| :--- | :--- |
| Reporting Format Statement | Coordinate for single point location. |
| Reporting Format Definition | This field is paired with "Latitude" to create a coordinate pair for a single point. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format. |
| Required, Recommended or Optional | optional |
| Format |  |

## Missing value codes

| Metadata Element | Missing\_Value\_Codes |
| :--- | :--- |
| Reporting Format Statement | Report missing value codes |
| Reporting Format Definition | Report all Missing Value Codes. For columns containing numeric data, use "-9999" as the missing value code \(or modify to match significant figures given the data\). For columns containing character data, use "N/A" as the missing value code. If entering more than one missing value code, use a vertical bar "|" or semicolon ";" instead of a comma or protect the comma with matching double quotation marks around the entire value. For more information about commas not meant to be a delimiter (e.g. used within a cell), refer to the Delimiter section of the CSV Reporting Format Detailed Guide. |
| Required, Recommended or Optional | optional |
| Format |  |

## Notes

| Metadata Element | Notes |
| :--- | :--- |
| Reporting Format Statement | Any information the provider would like to add. |
| Reporting Format Definition | Information provided would be data file specific. Details may include details on data file versioning, reporting format, software requirements, data quality, etc. |
| Required, Recommended or Optional | optional |
| Format |  |

## Field name orientation

| Metadata Element | Field\_Name\_Orientation |
| :--- | :--- |
| Reporting Format Statement | Orientation of the field name row or column. |
| Reporting Format Definition | Describe the orientation of the "Field Name" within the data matrix of the data file: 1\) Horizontal with field names at the top of columns or  2\) Vertical with field names starting rows. |
| Required, Recommended or Optional | optional |
| Format |  |


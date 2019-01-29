# Excel
## Populate Excel Template with CSV Data
### SYNOPSIS
```
    Populates a worksheet within an Excel template workbook with data specified in a CSV
```
### DESCRIPTION
```
    Given data represented in CSV format, this task will download a specified Excel template
    and populate a worksheet. Output will be the populated Excel template in Base64 encoded.
```
### INPUTS
```
    CsvString
        Single string (CSV format), required
        CSV data to populate a worksheet in the provided template
    ExcelXlsxTemplateFileUrl
        Single string (URL), required
        URL to the Excel template
    CsvDataWorksheetName
        Single string, optional.
        The name of the worksheet to populate the provided CSV data with. If no worksheet name
        has been provided, the system will create and populate a worksheet called 'data'
```
### OUTPUTS
```
    ExcelWorkbookBase64EncodedBytes
        Base64 encoded bytes
        Updated Excel template in Base64 encoded. To convert back to an Excel file, use 
        [Convert]::FromBase64String($ExcelWorkbookBase64EncodedBytes) | Set-Content -Encoding Byte -Path FILE_PATH
```
### NOTES
```
    Version: 1.0.1
    Last updated: 25 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


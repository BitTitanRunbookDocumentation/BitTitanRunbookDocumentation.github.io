# Excel
## Populate Excel Template with CSV Data
### SYNOPSIS
```
    Populates worksheets within an Excel template workbook with data specified in CSVs
```
### DESCRIPTION
```
    Given data represented in CSV format, this task will populate worksheets within the provided
    Excel workbook template. Output will be the populated Excel workbook Base64 encoded.
```
### INPUTS
```
    ExcelXlsxTemplateBase64EncodedBytes
        Base64 encoded bytes, required
        Excel template encoded in Base64 format
    Csv1String
        Single string (CSV format), required
        CSV data to populate a worksheet in the provided template
    CsvDataWorksheet1Name
        Single string, optional
        The name of the worksheet to populate the provided CSV data with. If no worksheet name
        has been provided, the system will create and populate a worksheet called 'data'
    Csv(X)String - Where (X) is 2, 3, 4 or 5
        Same as Csv1String, optional
    CsvDataWorksheet(X)Name - Where (X) is 2, 3, 4 or 5
        Same as CsvDataWorksheet1Name, optional
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
    Version: 2.0.0
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


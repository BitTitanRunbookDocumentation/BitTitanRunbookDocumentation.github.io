# Excel
## Convert To PDF
### SYNOPSIS
```
    Converts an Excel workbook to PDF format
```
### DESCRIPTION
```
    Converts a Base64 encoded Excel worksheet into a Base64 encoded PDF
```
### INPUTS
```
    ExcelWorkbook
        Base64 encoded bytes, using [Convert]::ToBase64String((Get-Content -Encoding Byte -Path <path>))
    WorksheetName
        Single string, optional
    CellRange
        Single string, optional
        Example:
            "A5" selects A5
            "A1:B3" selects A1, A2, A3, B1, B2, B3
```
### OUTPUTS
```
    Pdf
        Base64 encoded bytes
        To convert back to a pdf file, use [Convert]::FromBase64String($Pdf) | Set-Content -Encoding Byte -Path <path>
```
### NOTES
```
    Version: 1.1
    Last updated: 11 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


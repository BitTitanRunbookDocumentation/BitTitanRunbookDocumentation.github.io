# Excel
## Convert To HTML
### SYNOPSIS
```
    Converts an Excel worksheet to HTML format
```
### DESCRIPTION
```
    Converts a Base64 encoded Excel worksheet into HTML format as a string 
```
### INPUTS
```
    ExcelWorkbook
        Base64 encoded bytes, using [Convert]::ToBase64String((Get-Content -Encoding Byte -Path FILE_PATH))
    WorksheetName
        Single string, optional
```
### OUTPUTS
```
    Html
        A string representing the Excel worksheet in HTML format
```
### NOTES
```
    Version: 1.0
    Last updated: 08 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


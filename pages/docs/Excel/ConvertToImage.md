# Excel
## Convert To Image
### SYNOPSIS
```
    Converts an Excel workbook to an image format
```
### DESCRIPTION
```
    Converts a Base64 encoded Excel worksheet into a Base64 encoded image
```
### INPUTS
```
    ExcelWorkbook
        Base64 encoded bytes, using [Convert]::ToBase64String((Get-Content -Encoding Byte -Path <path>))
    WorksheetName
        Single string, optional
    ImageFormat
        Single string, optional, valid values are jpg, bmp, png, gif, jpeg, tiff. The default value is jpg
```
### OUTPUTS
```
    Image
        Base64 encoded bytes
        To convert back to a image file, use [Convert]::FromBase64String($Image) | Set-Content -Encoding Byte -Path <path>
```
### NOTES
```
    Version: 1.0
    Last updated: 08 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


# MSPComplete
## Compress Files
### SYNOPSIS
```
    Compresses one or more files into a zip archive
```
### DESCRIPTION
```
    Compresses one or more files into a zip archive.
    It:
        - Creates a temporary working folder
        - Creates copies of the files in the folder
        - Creates a zip file containing the files to compress in the folder
```
### INPUTS
```
    This task provides 5 pairs of File*Name and File*Contents (File1Name, File1Contents, etc...).
    File*Name
        Single string, in the format of 'name.extension'
        Examples: 'report.pdf', 'spreadsheet.xlsx'
    File*Contents
        The Base64 encoded byte content of the file.
```
### OUTPUTS
```
    ZipContents
        The Base64 encoded byte content of the zip file containing all the files to compress.
```
### NOTES
```
    Version: 1.0
    Last updated: 26 December 2018
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


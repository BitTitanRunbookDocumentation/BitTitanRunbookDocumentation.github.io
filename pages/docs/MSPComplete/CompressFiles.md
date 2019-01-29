# MSPComplete
## Compress Files
### SYNOPSIS
```
    Compresses up to five files into a zip archive with the option to password protect the archive
```
### DESCRIPTION
```
    Compresses up to five files into a zip archive with the option to password protect the archive.
    If the file is in text format (i.e. extension with txt, csv, log, bat, dat), no encoding of the
    file is required.
    Otherwise if the file is not in text format, the file bytes are to be encoded in Base64.
```
### INPUTS
```
    File1Name
        A single string, in the format of FILENAME.EXTENSION, required.
        Examples: report.pdf
    File1Contents
        A single string, required.
        If the file is in text format, this should be the text contents of the file.
        If the file is in non-text format, the contents should be the Base64 encoded byte contents
        of the file, using [Convert]::ToBase64String((Get-Content -Encoding Byte -Path FILE_PATH)).
    File(X)Name - Where (X) is 2, 3, 4 or 5
        Same as File1Name, optional
    File(x)Contents - Where (X) is 2, 3, 4 or 5
        Same as File1Contents, optional
    Password
        A single string, optional.
        If provided, this password protects the zip archive.
```
### OUTPUTS
```
    ZipContents
        The Base64 encoded byte content of the zip file containing all the files to compress.
        To convert back to a zip file, use:
            [Convert]::FromBase64String($ZipContents) | Set-Content -Encoding Byte -Path FILE_PATH
```
### NOTES
```
    Version: 1.1
    Last updated: 28 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


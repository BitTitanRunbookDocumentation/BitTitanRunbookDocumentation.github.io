# MSPComplete
## Decompress Files
### SYNOPSIS
```
    Decompresses a zip archive and returns up to five of the files contained in the archive
```
### DESCRIPTION
```
    Decompresses a zip archive and returns up to five of the files contained in the archive
    Specific file paths may be specified within the archive to select the files to be returned.
    If the file paths are not specified, the first five files in the archive will be returned,
    when sorted by file name.
```
### INPUTS
```
    Usage option 1: Decompress a zip archive and return up to the first five files in the archive,
                    sorted by file name
        ZipContents
            A single string, required.
            This is the Base64 encoded byte contents of the zip archive. To generate this, use
            [Convert]::ToBase64String((Get-Content -Encoding Byte -Path ZIP_FILE_PATH)).
        Password
            A single string, optional.
            This specifies the password used to decompress the zip archive, if it is password protected.
    Usage option 2: Decompress a zip archive and return up to the five files specified by their relative file paths
        ZipContents
            A single string, required.
            This is the Base64 encoded byte contents of the zip archive. To generate this, use:
                [Convert]::ToBase64String((Get-Content -Encoding Byte -Path ZIP_FILE_PATH)).
        Password
            A single string, optional.
            This specifies the password used to decompress the zip archive, if it is password protected.
        FilePathsToReturn
            Up to five strings separated by a newline, required.
            This specifies up to five files within the zip archive which will be returned by this task.
            The file paths are relative to the root directory of the archive.
```
### OUTPUTS
```
    MSPCompleteDecompressFilesFile(X)Name - Where (X) is 1, 2, 3, 4 or 5
        The name of each of the files returned by this task.
    MSPCompleteDecompressFilesFile(X)Contents - Where (X) is 1, 2, 3, 4 or 5
        If the returned file is in text format, this is the text contents of the file.
        Otherwise, this is the Base64 encoded byte contents of the file. To convert the byte
        contents back to a file, use:
            [Convert]::FromBase64String($MSPCompleteDecompressFilesFile(X)Contents) | Set-Content -Encoding Byte -Path OUTPUT_FILE_PATH
```
### NOTES
```
    Version: 1.0.1
    Last updated: 8 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


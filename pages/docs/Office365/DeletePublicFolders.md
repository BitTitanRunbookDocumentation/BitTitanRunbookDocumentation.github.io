# Office 365
## Delete Public Folders
### SYNOPSIS
```
    Delete Office 365 Public Folders
```
### DESCRIPTION
```
    The task library component deletes public folders from an input list of identities.
    An identity is the full path of the public folder, e.g. "\Test\Directory\My Public Folder".
    To prevent the accidental removal of sub-folders, all sub-folders must be specified in the identity list before the parent folder.
```
### INPUTS
```
    Usage option: Delete a list of Public Folders
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        PublicFolderIdentities
            A list of Public Folder full paths separated by newline, required.
            Example:
                \Test\Directory\My Public Folder 1\Folder 1-1
                \Test\Directory\My Public Folder 1\Folder 1-2
                \Test\Directory\My Public Folder 1
                \Test\Directory\My Public Folder 2
                \Test\Directory\My Public Folder 3
```
### OUTPUTS
```
    Office365DeletePublicFoldersAllErrorMessages
        A string containing all the error messages generated over the course of this task.
```
### NOTES
```
    Version: 1.0.2
    Last updated: 20 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


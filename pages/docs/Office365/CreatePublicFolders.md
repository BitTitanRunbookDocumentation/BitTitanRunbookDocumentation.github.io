# Office 365
## Create Public Folders
### SYNOPSIS
```
    Create Public Folders
```
### DESCRIPTION
```
    The task library component creates a Public Folder with the provided name and path.
    It also creates a group of Public Folders from the inputs in a CSV file
```
### INPUTS
```
    Usage option 1: Create a Public Folder
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        PublicFolderName
            A string representing the name of the Public Folder, required.
            Example: Marketing
        PublicFolderMailbox
            A string representing the identity of the hierarchy public folder mailbox, optional.
            Example: Primary Hierarchy Mailbox
        PublicFolderPath
            A string representing the path of the Public Folder, optional.
            The path must start with a \.
            Example: \Marketing
    Usage option 2: Create a group of Public Folders, using the inputs from a CSV file
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        PublicFoldersCsv
            PublicFolderName
                A string representing the name of the Public Folder, required.
                Example: Marketing
            PublicFolderMailbox
                A string representing the identity of the hierarchy public folder mailbox, optional.
                Example: Primary Hierarchy Mailbox
            PublicFolderPath
                A string representing the path of the Public Folder, optional.
                The path must start with a \.
                Example: \Marketing
```
### OUTPUTS
```
    Office365CreatePublicFoldersAllErrorMessages
        A string containing all the error messages generated over the course of this task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 31 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


# MigrationWiz
## Add Users to Project
### SYNOPSIS
```
    Adds users to a MigrationWiz mailbox migration project
```
### DESCRIPTION
```
    Adds users to a MigrationWiz mailbox migration project
```
### INPUTS
```
    Usage option 1: Add MSPComplete end users to a MigrationWiz mailbox migration project
        Users
            One or more MSPComplete end user objects, required.
            These are the users which will be added to the project.
        ProjectName
            A single string, optional. Either this or ConnectorId must be provided.
            This is the name of the mailbox migration project.
        ConnectorId
            A single string, optional. Either this or ProjectName must be provided.
            This is the connector ID of the mailbox migration project.
    Usage option 2: Add users to a MigrationWiz mailbox migration project using a CSV string
        UsersInformationCsv
            A CSV string containing information about the users to add to the project.
            Required columns:
                UserPrincipalName
                    A single string.
                    This is the user principal name of the user to add to the project.
        ProjectName
            A single string, optional. Either this or ConnectorId must be provided.
            This is the name of the mailbox migration project.
        ConnectorId
            A single string, optional. Either this or ProjectName must be provided.
            This is the connector ID of the mailbox migration project connector.
```
### OUTPUTS
```
    None
```
### NOTES
```
    Version: 1.1.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


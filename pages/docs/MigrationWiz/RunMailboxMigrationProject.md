# MigrationWiz
## Run Mailbox Migration Project
### SYNOPSIS
```
    Runs a mailbox migration project
```
### DESCRIPTION
```
    Runs a mailbox migration project
```
### INPUTS
```
    ExecutionType
        A single string, required, valid values are 'Verify Credentials', 'Trial Migration', 'Pre-Stage Migration', 'Full Migration' and 'Retry Errors'.
        This specifies the type of execution which will be run for the migration project.
    ProjectName
        A single string, optional. Either this or ConnectorId must be provided.
        This is the name of the mailbox migration project.
    ConnectorId
        A single string, optional. Either this or ProjectName must be provided.
        This is the connector ID of the mailbox migration project.
    Users
        One or more MSPComplete end user objects, optional.
        These are the users for which the project will be executed.
        If this is not provided, all mailboxes will be loaded from the project.
    PreStageDays
        A single string, optional.
        This specifies the cutoff date for items for a Pre-Stage migration.
    ItemTypes
        One or more strings separated by a comma, optional. Valid values are 'Contact', 'Calendar', 'Mail', 'Journal', 'Note', 'Task' and 'Rule'.
        This specifies the types of items which will be handled by the migration project when run.
```
### OUTPUTS
```
    None
```
### NOTES
```
    Version: 1.0.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


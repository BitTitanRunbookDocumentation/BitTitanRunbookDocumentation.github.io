# Active Directory
## Import Users Into MSPComplete
### SYNOPSIS
```
    Imports all users from Active Directory into MSPComplete
```
### DESCRIPTION
```
    Imports all users from Active Directory into MSPComplete.
    The users will be imported into the current MSPComplete customer in context.
```
### INPUTS
```
    Filter
        A single string, optional, defaults to "*"
        This filter will select which of the users retrieved from Active Directory will be imported into MSPComplete.
        For more information on how to use this, type "Get-Help about_ActiveDirectory_Filter" or see https://docs.microsoft.com/en-us/powershell/module/addsadministration/get-aduser?view=win10-ps.
    CreateUsers
        A single boolean value, optional, defaults to true.
        Selects whether a user should be created in MSPComplete if it does not exist in MSPComplete, but if it exists in Active Directory.
    UpdateUsers
        A single boolean value, optional, defaults to true.
        Selects whether a user should be updated in MSPComplete to match the user in Active Directory, if it exists in both MSPComplete and Active Directory.
    DeleteUsers
        A single boolean value, optional, defaults to false.
        Selects whether a users should be deleted from MSPComplete if it exists in MSPComplete, but not in Active Directory.
```
### OUTPUTS
```
    ActiveDirectoryImportUsersIntoMSPCompleteErrorMessages
        A string containing the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


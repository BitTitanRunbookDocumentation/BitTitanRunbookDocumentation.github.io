# Active Directory
## Delete Users
### SYNOPSIS
```
    Deletes one or more users in Active Directory
```
### DESCRIPTION
```
    Deletes one or more users in Active Directory
```
### INPUTS
```
    Users
        One or more MSPComplete end user objects, required.
        These users will be deleted from Active Directory.
        The user objects need to have an 'OnPremisesSecurityIdentifier' extended property, which corresponds to the 'objectSID' or 'SID' property on the Active Directory user.
```
### OUTPUTS
```
    ActiveDirectoryDeleteUsersErrorMessages
        A string containing the error messages which were generated over the course of the task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


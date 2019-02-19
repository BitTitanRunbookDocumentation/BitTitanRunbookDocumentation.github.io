# Office 365
## Grant/Remove Send As Permissions
### SYNOPSIS
```
    Grants or removes 'Send As' Permission to mailboxes, distribution groups or dynamic distribution groups
```
### DESCRIPTION
```
    Grants or removes 'Send As' Permission to mailboxes, distribution groups or dynamic distribution groups
```
### INPUTS
```
    Usage option 1: Grant or remove one user's 'Send As' Permission to multiple user mailboxes
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        GranteeUsers
            Single MSPComplete end user object, required.
        GrantorUsers
            Multiple MSPComplete end user objects, required.
        GrantOrRemovePermission
            A single string, required.
            Valid values are 'grant' and 'remove' (case-insensitive).
    Usage option 2: Grant or remove multiple users' 'Send As' Permission to one user mailbox
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        GranteeUsers
            Multiple MSPComplete end user objects, required.
        GrantorUsers
            Single MSPComplete end user object, required.
            If more than one object is provided, only the first one is used
        GrantOrRemovePermission
            A single string, required.
            Valid values are 'grant' and 'remove' (case-insensitive).
    Usage option 3: Grant or remove one user's 'Send As' Permission to multiple group mailboxes
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        GranteeUsers
            Single MSPComplete end user object, required.
        GrantorGroups
            Multiple MSPComplete group objects, required.
        GrantOrRemovePermission
            A single string, required.
            Valid values are 'grant' and 'remove' (case-insensitive).
    Usage option 4: Grant or remove one user's 'Send As' Permission to multiple group mailboxes
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        GranteeUsers
            Multiple MSPComplete end user objects, required.
        GrantorGroups
            Single MSPComplete group object, required.
            If more than one object is provided, only the first one is used.
        GrantOrRemovePermission
            A single string, required.
            Valid values are 'grant' and 'remove' (case-insensitive).
    Usage option 5: Grant or remove 'Send As' Permissions via CSV
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        SendAsPermissionsCsv
            Required columns:
                GranteeEmailAddress
                    The email address of the grantee.
                GrantOrRemovePermission
                    Valid values are 'grant' and 'remove' (case-insensitive).
                GrantorEmailAddress
                    The email address of the grantor.
```
### OUTPUTS
```
    Office365GrantRemoveSendAsPermissionsCsv
        A CSV containing all the users and groups which were processed by this task, as well as an additional
        column 'UpdatedPermission' to indicate if the change of permission is successful.
    Office365GrantRemoveSendAsPermissionsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0
    Last updated: 13 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


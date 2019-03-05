# Office 365
## Grant/Remove Send On Behalf Permissions
### SYNOPSIS
```
    Grants or removes 'Send On Behalf' Permission for mailboxes, distribution groups to mailboxes, distribution groups or dynamic distribution groups
```
### DESCRIPTION
```
    Grants or removes 'Send On Behalf' Permission for mailboxes, distribution groups to mailboxes, distribution groups or dynamic distribution groups
```
### INPUTS
```
    Usage option 1: Grant or remove one (user or group)'s 'Send On Behalf' Permission to multiple (user and group) mailboxes
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        GranteeUsers
            Single MSPComplete end user object, required.
        GranteeGroups
            Single MSPComplete group object, required.
        GrantorUsers
            Multiple MSPComplete end user objects, required.
        GrantorGroups
            Multiple MSPComplete group objects, required.
        GrantOrRemovePermission
            A single string, required.
            Valid values are 'grant' and 'remove' (case-insensitive).
    Usage option 2: Grant or remove multiple (user and group)s' 'Send On Behalf' Permission to one (user or group) mailbox
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        GranteeUsers
            Multiple MSPComplete end user objects, required.
        GranteeGroups
            Multiple MSPComplete group objects, required.
        GrantorUsers
            Single MSPComplete end user object, required.
            If more than one object is provided, only the first one is used
        GrantorGroups
            Single MSPComplete group object, required.
            If more than one object is provided, only the first one is used
        GrantOrRemovePermission
            A single string, required.
            Valid values are 'grant' and 'remove' (case-insensitive).
    Usage option 3: Grant or remove 'Send On Behalf' Permissions via CSV
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        SendOnBehalfOfPermissionsCsv
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
    Office365GrantRemoveSendOnBehalfPermissionsCsv
        A CSV containing all the users and groups which were processed by this task, as well as an additional
        column 'UpdatedPermission' to indicate if the change of permission is successful.
    Office365GrantRemoveSendOnBehalfPermissionsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0
    Last updated: 28 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


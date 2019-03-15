# Active Directory
## Add/Remove Users From Groups
### SYNOPSIS
```
    Adds or removes users from groups in Active Directory
```
### DESCRIPTION
```
    Adds or removes users from groups in Active Directory
```
### INPUTS
```
    Usage option 1: Add or remove a user from one or more groups
        Users
            A single MSPComplete end user object, required.
            This is the user in Active Directory which will be added or removed from the groups.
            The user object is required have an 'OnPremisesSecurityIdentifier' extended property, which corresponds to the 'objectSID' or 'SID' property on the Active Directory user.
        GroupIdentities
            One or more strings separated by a newline, required.
            This identifies the groups which the user will be added/removed from.
            The identity of the group can be:
                - A distinguished name
                - A GUID (the objectGUID property)
                - A security identifier (the objectSid property)
                - A SAM account name (the sAMAccountName property)
        AddOrRemoveUser
            A single string, required, valid values are 'add' and 'remove' (case-insensitive).
            This specifies if the user will be added or removed from all of the groups.
    Usage option 2: Add or remove one or more users from one group
        Users
            One or more MSPComplete end user objects, required.
            These are the users in Active Directory which will be added or removed from the groups.
            The user objects are required have an 'OnPremisesSecurityIdentifier' extended property, which corresponds to the 'objectSID' or 'SID' property on the Active Directory user.
        GroupIdentities
            A single string, required.
            This identifies the group which the users will be added/removed from.
            The identity of the group can be:
                - A distinguished name
                - A GUID (the objectGUID property)
                - A security identifier (the objectSid property)
                - A SAM account name (the sAMAccountName property)
        AddOrRemoveUser
            A single string, required, valid values are 'add' and 'remove' (case-insensitive).
            This specifies if the users will be added or removed from the group.
    Usage option 3: Add or remove users from groups
        UsersCsv
            A CSV string containing information about the users to be added/removed from groups.
            Required columns:
                UserIdentity
                    A single string.
                    This identifies the user which will be added/removed from the group.
                    The identity of the user can be:
                        - A distinguished name
                        - A GUID (the objectGUID property)
                        - A security identifier (the objectSid property)
                        - A SAM account name (the sAMAccountName property)
                GroupIdentity
                    A single string.
                    This identifies the group which the user will be added/removed from.
                    The identity of the group can be:
                        - A distinguished name
                        - A GUID (the objectGUID property)
                        - A security identifier (the objectSid property)
                        - A SAM account name (the sAMAccountName property)
                AddOrRemoveUser
                    A single string, required, valid values are 'add' and 'remove' (case-insensitive).
                    This specifies if the user will be added or removed from the group.
```
### OUTPUTS
```
    ActiveDirectoryAddRemoveUsersFromGroupsCsv
        A CSV string containing information about the users which were added/removed from the groups, as well as an additional column 'MembershipUpdated' to indicate if the users were successfully added/removed from the groups.
    ActiveDirectoryAddRemoveUsersFromGroupsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 2.0.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


# Active Directory
## Enable/Disable User Accounts
### SYNOPSIS
```
    Enables or disables one or more user accounts in Active Directory
```
### DESCRIPTION
```
    Enables or disables one or more user accounts in Active Directory
```
### INPUTS
```
    Usage option 1: enables or disables one or more user accounts in Active Directory
        Users
            One or more MSPComplete end user objects, required.
            The user objects need to have a 'OnPremisesSecurityIdentifier' extended property, which is the
            users' identities in Active Directory.
        EnableOrDisableAccount
            A single string, required, valid values are 'enable' and 'disable' (case-insensitive).
            This specifies if the user will be enabled or disabled.
    Usage option 2: enables or disables one or more user accounts in Active Directory via CSV
        UsersCsv
            A CSV string containing information about the users to enabled or disabled.
            Required columns:
                Identity
                    A single string.
                    This identifies the user which will be enabled or disabled.
                    The identity of the user can be:
                        - A distinguished name
                        - A GUID (the objectGUID property)
                        - A security identifier (the objectSid property)
                        - A SAM account name (the sAMAccountName property)
                EnableOrDisableAccount
                    A single string, required, valid values are 'enable' and 'disable' (case-insensitive).
                    This specifies if the user will be enabled or disabled.
```
### OUTPUTS
```
    ActiveDirectoryEnableDisableUserAccountsCsv
        A CSV string containing information about the users which were enabled or disabled,
        as well as an additional column 'UserUpdated' to indicate if the users were successfully
        enabled or disabled.
    ActiveDirectoryEnableDisableUserAccountsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0
    Last updated: 15 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


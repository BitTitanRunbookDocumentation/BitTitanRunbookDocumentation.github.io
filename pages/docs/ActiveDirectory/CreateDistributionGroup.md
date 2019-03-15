# Active Directory
## Create Distribution Group
### SYNOPSIS
```
    Creates a distribution group in Active Directory
```
### DESCRIPTION
```
    Creates a distribution group in Active Directory
```
### INPUTS
```
    DisplayName
        A single string, required.
        This is the display name of the group which will be created.
    GroupScope
        A single string, required, valid values are 'DomainLocal', 'Global' and 'Universal'.
        This is the scope of the group.
    Description
        A single string, optional.
        This is the description of the group.
    Email
        A single string, optional.
        This is the email address of the group.
    Owner
        A single string, optional.
        This specifies the user or group which will manage this new group.
        Possible identifiers are:
            - A distinguished name
            - A GUID (the objectGUID property)
            - A security identifier (the objectSid property)
            - A SAM account name (the sAMAccountName property)
    Path
        A single string, optional.
        This specifies the path of the Organizational Unit or container where the group will be created.
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


# Active Directory
## Wait For Group Azure AD Replication
### SYNOPSIS
```
    Waits for an Active Directory group to be replicated to Azure AD
```
### DESCRIPTION
```
    Waits for an Active Directory group to be replicated to Azure AD
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    Identity
        A single string, required.
        This specifies the group which is currently being waited upon for replication.
        The identity of the group can be:
            - A distinguished name
            - A GUID (the objectGUID property)
            - A security identifier (the objectSid property)
            - A SAM account name (the sAMAccountName property)
    MaximumWaitTimeMinutes
        A single string, optional, defaults to "15"
        This specifies the maximum amount of time this task will wait for the group to be replicated,
        in minutes.
```
### OUTPUTS
```

```
### NOTES
```
    Version: 1.0.1
    Last updated: 28 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


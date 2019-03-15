# Microsoft Teams
## Remove Users From Team
### SYNOPSIS
```
    (BETA) Removes one or more users from a team on Microsoft Teams
```
### DESCRIPTION
```
    (BETA) Removes one or more users from a team on Microsoft Teams
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    User
        One or more MSPComplete end user objects, required.
        These are the users which will be removed from the team.
    TeamDisplayName
        A single string, optional. Either this or TeamGroupId must be provided.
        This is the display name of the team which the users will be removed from.
    TeamGroupId
        A single string, optional. Either this or TeamDisplayName must be provided.
        This is the group ID of the team which the users will be removed from.
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


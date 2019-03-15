# Microsoft Teams
## Update Team
### SYNOPSIS
```
    (BETA) Updates a team on Microsoft Teams
```
### DESCRIPTION
```
    (BETA) Updates a team on Microsoft Teams
    The properties which can be updated are:
        - Display name
        - Description
        - Visibility
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    TeamDisplayName
        A single string, optional. Either this or TeamGroupId must be provided.
        This is the display name of the team which will be updated.
    TeamGroupId
        A single string, optional. Either this or TeamDisplayName must be provided.
        This is the group ID of the team which will be updated.
    NewDisplayName
        A single string, optional.
        This is the new display name of the team.
    NewDescription
        A single string, optional.
        This is the new description of the team.
    NewTeamVisibility
        A single string, optional, valid values are 'Private' and 'Public'.
        This is the new visibility of the team.
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


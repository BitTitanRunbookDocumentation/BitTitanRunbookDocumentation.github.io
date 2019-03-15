# Microsoft Teams
## Create Team
### SYNOPSIS
```
    (BETA) Creates a team in Microsoft Teams
```
### DESCRIPTION
```
    (BETA) Creates a team in Microsoft Teams
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    TeamDisplayName
        A single string, required.
        This is the display name of the new team.
    TeamDescription
        A single string, optional.
        This is the description of the new team.
    TeamVisibility
        A single string, optional, valid values are 'Private' and 'Public'.
        This the visibility of the new team.
    AddCreatorAsMember
        A single boolean value, optional, defaults to false.
        This specifies if the creator of the team (the Administrator) should be added as a member of the team.
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


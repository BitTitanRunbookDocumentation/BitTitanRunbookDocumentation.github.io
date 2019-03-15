# Microsoft Teams
## Add Users To Team
### SYNOPSIS
```
    (BETA) Adds one or more users to a team on Microsoft Teams
```
### DESCRIPTION
```
    (BETA) Adds one or more users to a team on Microsoft Teams
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    User
        One or more MSPComplete user objects, required.
        These are the users which will be added to the team.
    TeamDisplayName
        A single string, optional. Either this or TeamGroupId must be provided.
        This is the display name of the team which the users will be added to.
    TeamGroupId
        A single string, optional. Either this or TeamDisplayName must be provided.
        This is the group ID of the team which the users will be added to.
    Role
        A single string, optional.
        This specifies the roles which will be applied to the users within the team.
```
### OUTPUTS
```
    AllErrorMessages
        A string containing the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


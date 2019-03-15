# Microsoft Teams
## Retrieve Team Channels
### SYNOPSIS
```
    (BETA) Retrieves information about the channels within a team on Microsoft Teams
```
### DESCRIPTION
```
    (BETA) Retrieves information about the channels within a team on Microsoft Teams.
    Information retrieved about the channels are:
        - The channel ID
        - The channel display name
        - The channel description
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    TeamDisplayName
        A single string, optional. Either this or TeamGroupId must be provided.
        This is the display name of the team which the information will be retrieved from.
    TeamGroupId
        A single string, optional. Either this or TeamDisplayName must be provided.
        This is the group ID of the team which the information will be retrieved from.
```
### OUTPUTS
```
    TeamChannelsCsv
        A CSV string containing information about the channels within the team.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


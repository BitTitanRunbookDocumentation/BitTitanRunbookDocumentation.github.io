# Microsoft Teams
## Update Team Channel
### SYNOPSIS
```
    (BETA) Updates a channel within a team on Microsoft Teams
```
### DESCRIPTION
```
    (BETA) Updates a channel within a team on Microsoft Teams
    The properties which can be updated are:
        - Display name
        - Description
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    ChannelDisplayName
        A single string, required.
        This is the display name of the channel which will be updated.
    TeamDisplayName
        A single string, optional. Either this or TeamGroupId must be provided.
        This is the display name of the team which contains the channel which will be updated.
    TeamGroupId
        A single string, optional. Either this or TeamDisplayName must be provided.
        This is the group ID of the team which contains the channel which will be updated.
    NewChannelDisplayName
        A single string, optional.
        This is the new display name of the channel.
    NewChannelDescription
        A single string, optional.
        This is the new description of the channel.
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


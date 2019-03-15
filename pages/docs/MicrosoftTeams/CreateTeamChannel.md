# Microsoft Teams
## Create Team Channel
### SYNOPSIS
```
    (BETA) Creates a channel within a team in Microsoft Teams
```
### DESCRIPTION
```
    (BETA) Creates a channel within a team in Microsoft Teams
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    ChannelDisplayName
        A single string, required.
        This is the display name of the new channel.
    TeamDisplayName
        A single string, optional. Either this or TeamGroupId must be provided.
        This is the display name of the team in which the channel will be created.
    TeamGroupId
        A single string, optional. Either this or TeamDisplayName must be provided.
        This is the group ID of the team in which the channel will be created.
    ChannelDescription
        A single string, optional.
        This is the description of the new channel.
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


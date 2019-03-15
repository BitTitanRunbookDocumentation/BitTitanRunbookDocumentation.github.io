# Microsoft Teams
## Delete Team Channel
### SYNOPSIS
```
    (BETA) Deletes a channel within a team on Microsoft Teams
```
### DESCRIPTION
```
    (BETA) Deletes a channel within a team on Microsoft Teams
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    ChannelDisplayName
        A single string, required.
        This is the display name of the channel which will be deleted.
    TeamDisplayName
        A single string, optional. Either this or TeamGroupId must be provided.
        This is the display name of the team which the channel belongs to.
    TeamGroupId
        A single string, optional. Either this or TeamDisplayName must be provided.
        This is the group ID of the team which the channel belongs to.
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


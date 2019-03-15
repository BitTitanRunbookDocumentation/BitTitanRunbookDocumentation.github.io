# Microsoft Teams
## Retrieve Teams
### SYNOPSIS
```
    (BETA) Retrieves information about teams in Microsoft Teams
```
### DESCRIPTION
```
    (BETA) Retrieves information about teams in Microsoft Teams.
    Information retrieved about the teams are:
        - The team group ID
        - The team display name
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    TeamDisplayNames
        One or more strings separated by a newline, optional.
        This specifies the display names of the teams to retrieve information about.
```
### OUTPUTS
```
    TeamsCsv
        A CSV string containing information about the teams.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


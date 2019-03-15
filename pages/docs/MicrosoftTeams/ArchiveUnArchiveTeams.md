# Microsoft Teams
## Archive/Unarchive Teams
### SYNOPSIS
```
    (BETA) Archives/Unarchives one or more teams on Microsoft Teams
```
### DESCRIPTION
```
    (BETA) Archives/Unarchives one or more teams on Microsoft Teams
```
### INPUTS
```
    Usage option 1: Archive/unarchive a team
        MicrosoftGraphCredentials
            A MSPComplete endpoint object containing the Microsoft Graph credentials, required.
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        TeamDisplayName
            A single string, required.
            This specifies the display name of the team to archive or unarchive.
        ArchiveOrUnarchive
            A single string, required, valid values are "Archive" and "Unarchive" (case-insensitive).
        MaximumWaitTimeMinutes
            A single string, optional, defaults to 30.
            This specifies the maximum amount of time in minutes to wait for the archive/unarchive operation to be completed.
    Usage option 2: Archive/unarchive teams
        MicrosoftGraphCredentials
            A MSPComplete endpoint object containing the Microsoft Graph credentials, required.
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        TeamsCsv
            A CSV string containing information about the teams to archive/unarchive.
            Required columns:
                TeamDisplayName
                    A single string.
                    This specifies the display name of the team to archive or unarchive.
                ArchiveOrUnarchive
                    A single string, valid values are "Archive" and "Unarchive" (case-insensitive).
        MaximumWaitTimeMinutes
            A single string, optional, defaults to 30.
            This specifies the maximum amount of time in minutes to wait for the archive/unarchive operation to be completed.
```
### OUTPUTS
```
    MicrosoftTeamsArchiveUnarchiveTeamsCsv
        A CSV string containing information about the teams which were archived/unarchived, as well as an additional column "OperationSuccessful" to indicate if the archive/unarchive operation was successful.
    MicrosoftTeamsArchiveUnarchiveTeamsErrorMessages
        A string containing the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


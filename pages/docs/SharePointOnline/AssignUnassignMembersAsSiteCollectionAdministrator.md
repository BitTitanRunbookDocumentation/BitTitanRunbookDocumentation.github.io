# SharePoint Online
## Assign/Unassign Members as Site Collection Administrator
### SYNOPSIS
```
    Assigns or unassigns Site Collection members as Administrators
```
### DESCRIPTION
```
    Assigns or unassigns one or more users as Site Collection Administrator for a site or assigns and
    unassigns users as Site Collection Administrator for SharePoint Online sites via a CSV
```
### INPUTS
```
    Usage option 1: Assigns or unassigns one or more users as Site Collection Administrator
    for a specified SharePoint Online site
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        Users
            One or more MSPComplete user objects, required
        Url
            Single string, required
            The URL of the SharePoint Online site to assign/unassign
            Site Collection Administrators
        IsSiteCollectionAdmin
            Single bool, required
            True to assign as an administrator, false to unassign
    Usage option 2: Assigns and unassigns users as Site Collection Administrator for SharePoint
    Online sites using a CSV
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        UsersCsv
            Required columns:
                PrimaryEmailAddress
                    The primary email address uniquely identifying an user
                Url
                    The URL of the SharePoint Online site
                IsSiteCollectionAdmin
                    Either 'true' to assign user as an administrator or 'false' to unassign
```
### OUTPUT
```
    SharePointOnlineAssignUnassignMembersAsSiteCollectionAdministratorProcessedUsersCsv
        A CSV string containing the information about which users were successfully assigned or
        unassigned via an additional column 'Updated'.
    SharePointOnlineAssignUnassignMembersAsSiteCollectionAdministratorErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.2
    Last updated: 21 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


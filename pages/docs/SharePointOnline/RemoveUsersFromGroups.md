# SharePoint Online
## Remove Users From Groups
### SYNOPSIS
```
    Removes users from groups in SharePoint Online site collections
```
### DESCRIPTION
```
    Removes users from a group or users from multiple groups using a CSV
```
### INPUTS
```
    Usage option 1: Removes one or more users from a group
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        Users
            One or more MSPComplete user objects, required
        GroupName
            Single string, required
            The name of the group
        Url
            Single string, required.
            The URL of the SharePoint Online site collection
    Usage option 2: Removes users from multiple groups using a CSV
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        UsersCsv
            Required columns:
                PrimaryEmailAddress
                    The primary email address uniquely identifying an user
                GroupName
                    The name of the group
                Url
                    The URL of the SharePoint Online site collection
```
### OUTPUTS
```
    SharePointOnlineRemovedUsersFromGroupsProcessedUsersCsv
        A CSV string containing the information about which users were successfully removed from the specified groups via an additional column 'RemovedFromGroup'.
    SharePointOnlineRemovedUsersFromGroupsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


# SharePoint Online
## Delete Groups
### SYNOPSIS
```
    Deletes groups in SharePoint Online site collections
```
### DESCRIPTION
```
    Delete a SharePoint Online site collection group or groups from
    specified SharePoint Online site collections via CSV format
```
### INPUTS
```
    Usage option 1: Delete a SharePoint Online site collection group
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        GroupName
            Single string, required
            The name of the SharePoint Online group to delete
        Url
            Single string, required.
            The URL of the SharePoint Online site to delete the group from
    Usage option 2: Delete groups from the specified SharePoint Online site collections
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        GroupsCsv
            Required columns:
                GroupName
                    The name of the SharePoint Online group to delete
                Url
                    The URL of the SharePoint Online site to delete the group from
```
### OUTPUTS
```
    SharePointOnlineDeleteGroupsProcessedGroupsCsv
        A CSV string containing the information about which groups were successfully deleted
        via an additional column 'Deleted'.
    SharePointOnlineDeleteGroupsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.2
    Last updated: 22 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


# SharePoint Online
## Create Groups
### SYNOPSIS
```
    Creates groups in SharePoint Online site collections
```
### DESCRIPTION
```
    Create a group with owner for a SharePoint Online site or create groups with owners for SharePoint Online sites via CSV format
```
### INPUTS
```
    Usage option 1: Create a group with owner for a SharePoint Online site collection
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        Url
            Single string, required.
            The URL of the SharePoint Online site collection to create the group in
        GroupName
            Single string, required
            The name of the SharePoint Online group
        GroupOwner
            Single MSPComplete user object, optional
            The user to be set as the owner of the SharePoint Online group
        PermissionLevels
            One or more strings, separated by a newline, required
            The permissions for the SharePoint Online group. The possible values are Full Control,
            Design, Edit, Contribute and Read
    Usage option 2: Create groups with owners for SharePoint Online sites
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        GroupsCsv
            Required columns:
                Url
                    The URL of the SharePoint Online site collection
                GroupName
                    The name of the SharePoint Online group to create
                PermissionLevels
                    The permissions given to the group, with each permission separated by commas and
                    enclosed in quotation marks, e.g. "Contribute, Read"
                    The possible permission levels are Full Control, Design, Edit, Contribute and Read
            Optional columns:
                GroupOwnerPrimaryEmailAddress
                    The primary email address uniquely identifying an user to be set as group owner
```
### OUTPUTS
```
    SharePointOnlineCreateGroupsProcessedGroupsCsv
        A CSV string containing the information about which groups were successfully created via an additional column 'Created'.
    SharePointOnlineCreateGroupsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


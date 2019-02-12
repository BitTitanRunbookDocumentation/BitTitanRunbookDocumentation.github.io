# SharePoint Online
## Add Users To Groups
### SYNOPSIS
```
    Adds users to groups in SharePoint Online site collections
```
### DESCRIPTION
```
    Adds users into a group or users into multiple groups using a CSV
```
### INPUTS
```
    Usage option 1: Add one or more users into a group
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
            The OrganizationName extended property is required - it is the portion of the domain before the '.onmicrosoft.com'
            Example: If the full domain is 'contoso.onmicrosoft.com', the OrganizationName is 'contoso'.
        Users
            One or more MSPComplete user objects, required.
            The users to add to the specified SharePoint Online site collection group
        GroupName
            Single string, required.
            The name of the group
        Url
            Single string, required.
            The URL of the SharePoint Online site collection
    Usage option 2: Add users into multiple groups using a CSV
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
            The OrganizationName extended property is required - it is the portion of the domain before the '.onmicrosoft.com'
            Example: If the full domain is 'contoso.onmicrosoft.com', the OrganizationName is 'contoso'.
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
    SharePointOnlineAddUsersToGroupsProcessedUsersCsv
        A CSV string containing the information about which users were successfully added to the
        specified groups via an additional column 'AddedToGroup'.
    SharePointOnlineAddUsersToGroupsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1
    Last updated: 16 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


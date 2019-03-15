# SharePoint Online
## Retrieve Groups
### SYNOPSIS
```
    Retrieves information about groups in SharePoint Online site collections as a CSV string
```
### DESCRIPTION
```
    Retrieves login, title, owner, users and role information in CSV format for a group or for groups in site collections using a CSV
```
### INPUTS
```
    Usage option 1: Retrieve information for a group
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        GroupName
            Single string, required
            The name of the group
        Url
            Single string, required
            The URL of the SharePoint Online site collection
    Usage option 2: Retrieve information for groups in specified site collections
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        GroupsCsv
            Required columns:
                GroupName
                    The name of the group
                Url
                    The URL of the SharePoint Online site collection
```
### OUTPUTS
```
    SharePointOnlineGroupPropertiesCsv
        CSV containing the Login name, title, owner, user and role information of the group
    SharePointOnlineRetrieveGroupsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0.2
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


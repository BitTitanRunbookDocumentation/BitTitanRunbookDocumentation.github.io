# SharePoint Online
## Retrieve Users In Site Collections
### SYNOPSIS
```
    Retrieves SharePoint Online site collection users' information as a CSV string
```
### DESCRIPTION
```
    Retrieves SharePoint Online site collection users' information as a CSV string
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    Urls
        Multiple strings separated by newline, optional
        The URL of the SharePoint Online site collection
```
### OUTPUTS
```
    SharePointOnlineUsersCsv
        The list of users in the provided SharePoint Online site collection URLs
    SharePointOnlineRetrieveUsersInSiteCollectionsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1
    Last updated: 16 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


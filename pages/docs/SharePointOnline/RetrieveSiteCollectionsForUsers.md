# SharePoint Online
## Retrieve Site Collections For Users
### SYNOPSIS
```
    Retrieves SharePoint Online site collections containing the provided users
```
### DESCRIPTION
```
    Retrieves SharePoint Online site collections containing the provided users
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    Users
        One or more MSPComplete user objects, required
```
### OUTPUTS
```
    SharePointOnlineSiteCollectionsCsv
        The list of site collections that contain the provided users. Additional information include
        the URL, user's display name and email address and site collection group they belong in
    SharePointOnlineRetrieveSiteCollectionsForUsersErrorMessagessnipp
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 16 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


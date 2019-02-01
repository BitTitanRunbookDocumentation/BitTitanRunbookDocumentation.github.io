# SharePoint Online
## Retrieve Site Collections' Statistics
### SYNOPSIS
```
    Retrieves statistics about SharePoint Online site collections as a CSV string
```
### DESCRIPTION
```
    Retrieves statistics about SharePoint Online site collections as a CSV string
```
### INPUTS
```
    Usage option 1: Add one or more users into a group
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        Urls
            Multiple string values, separated by a newline, required.
            The URLs of the SharePoint Online site collections to retrieve statistics on
```
### OUTPUTS
```
    SharePointOnlineSiteCollectionsCsv
        A CSV string containing statistics about the provided SharePoint Online site collections
    SharePointOnlineRetrieveSiteCollectionsStatisticsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 16 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


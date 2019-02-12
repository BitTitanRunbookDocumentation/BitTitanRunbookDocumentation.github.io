# SharePoint Online
## Retrieve Deleted Site Collections
### SYNOPSIS
```
    Retrieves SharePoint Online site collections in the Recycle Bin as a CSV string
```
### DESCRIPTION
```
    Retrieves SharePoint Online site collections in the Recycle Bin as a CSV string
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    IncludePersonalSites
        Single bool, optional.
```
### OUTPUTS
```
    SharePointOnlineDeletedSiteCollectionsCsv
        CSV containing the URL, deletion time, days remaining and storage quota information of
        the deleted site collections
```
### NOTES
```
    Version: 1.0
    Last updated: 30 November 2018
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


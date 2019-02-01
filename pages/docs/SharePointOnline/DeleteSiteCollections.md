# SharePoint Online
## Delete Site Collections
### SYNOPSIS
```
    Deletes one or more site collections in SharePoint Online
```
### DESCRIPTION
```
    Deletes one or more site collections in SharePoint Online.
    By default, the site collections are moved to the Recycle Bin on SharePoint Online.
    If PermanentlyDelete is set to true, the site collections are permanently deleted from
    the Recycle Bin as well.
```
### INPUTS
```
    Usage option 1: Delete a SharePoint Online site collection
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        Url
            Single string, required.
            The URL of the SharePoint Online site collection to delete
        PermanentlyDelete
            Single bool, optional.
    Usage option 2: Delete SharePoint Online site collections
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        SiteCollectionsCsv
            Required columns:
                Url
                    The URL of the SharePoint Online site collection to delete
            Optional columns
                PermanentlyDelete
                    Valid values are 'true' or 'false'
```
### OUTPUTS
```
    SharePointOnlineDeleteSiteCollectionsProcessedSiteCollectionsCsv
        A CSV string containing the information about which site collections were successfully deleted
        via an additional column 'Deleted'.
    SharePointOnlineDeleteSiteCollectionsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1
    Last updated: 16 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


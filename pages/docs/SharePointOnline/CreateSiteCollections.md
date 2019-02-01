# SharePoint Online
## Create Site Collections
### SYNOPSIS
```
    Creates one or more site collections in SharePoint Online
```
### DESCRIPTION
```
    Creates a SharePoint Online site collection or multiple site collections via CSV format
```
### INPUTS
```
    Usage option 1: Create a SharePoint Online site collection
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        Owner
            Single MSPComplete user object, required.
            Owner for the SharePoint Online site collection
        CompatibilityLevel
            Single string, optional.
            Either 14 (Compatible with SharePoint 2010) or 15 (SharePoint 2013)
        LocaleId
            Single string, optional.
            The language for the site collection. Use cmdlet Get-SPOWebTemplate for the 
            list of valid combinations in conjunction with Template
        ResourceQuota
            Single string, optional.
            The quota for the site collection with default value set as 0. View Microsoft's
            documentation on New-SPOSite for more information
        StorageQuotaMegabytes
            Single string, required.
            The total storage size for the site collection in megabytes
        Template
            Single string, optional.
            The site collection template to use when creating the site. Use cmdlet Get-SPOWebTemplate 
            for the list of valid combinations in conjunction with LocaleId
        TimeZoneId
            Single string, optional.
            The time zone for the site collection
        Title
            Single string, optional.
            The title for the site collection
        Url
            Single string, required.
            The url for the site collection
    Usage option 2: Creates SharePoint Online site collections
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        SiteCollectionsCsv
            Required columns:
                OwnerPrimaryEmailAddress
                    Email address of the primary owner for the SharePoint Online site collection
                Url
                    The url for the site collection
                StorageQuotaMegabytes
                    The total storage size for the site collection in megabytes
            Optional columns:
                CompatibilityLevel
                    Either 14 (Compatible with SharePoint 2010) or 15 (SharePoint 2013)
                LocaleId
                    The language for the site collection. Use cmdlet Get-SPOWebTemplate for the list 
                    of valid combinations in conjunction with Template
                ResourceQuota
                    The quota for the site collection with default value set as 0. View Microsoft's
                    documentation on New-SPOSite for more information
                Template
                    The site collection template to use when creating the site. Use cmdlet 
                    Get-SPOWebTemplate for the list of valid combinations in conjunction with LocaleId
                TimeZoneId
                    The time zone for the site collection
                Title
                    The title for the site collection
```
### OUTPUTS
```
    SharePointOnlineCreateSiteCollectionsProcessedSiteCollectionsCsv
        A CSV string containing the information about which sites were successfully created 
        via an additional column 'Created'.
    SharePointOnlineCreateSiteCollectionsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1
    Last updated: 16 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


# SharePoint Online
## Update Site Collections' Sharing Settings
### SYNOPSIS
```
    Updates the sharing settings of one or more site collections in SharePoint Online
```
### DESCRIPTION
```
    Updates the sharing settings of one or more site collections in SharePoint Online.
    This task makes use of the Set-SPOSite cmdlet to update the various settings.
```
### INPUTS
```
    Usage option 1: Update the settings of a SharePoint Online site collection
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
            The OrganizationName extended property is required - it is the portion of the domain before the '.onmicrosoft.com'
            Example: If the full domain is 'contoso.onmicrosoft.com', the OrganizationName is 'contoso'.
        Url
            Single string, required.
            The URL of the SharePoint Online site collection
        DefaultLinkPermission
            Single string, optional.
            This sets the default link permission for the site collection.
            Possible values are 'None', 'View' and 'Edit'.
            This property is not modified if not specified.
            None - Respects the default organization link permission.
            View - The default link permission is 'view'.
            Edit - The default link permission is 'edit'.
        DefaultSharingLinkType
            Single string, optional.
            This sets the default link type for the site collection
            Possible values are 'None', 'AnonymousAccess', 'Internal' and 'Direct'.
            This property is not modified if not specified.
            None - Respects the default organization link type.
            AnonymousAccess - The default link type is 'Anonymous Access' or anyone.
            Internal - The default link type is 'Organization' or company shareable.
            Direct - The default link type is 'Specific People'.
        SharingAllowedDomainList
            One or more strings separated by a newline, optional.
            This specifies a list of email domains that are allowed as external collaborators.
            This property is not modified if not specified.
            To clear the existing list, use the value of $CLEAR_VALUE_FLAG as defined in BitTitan.Runbooks.Common.
        SharingBlockedDomainList
            One or more strings separated by a newline, optional.
            This specifies a list of email domains that are blocked as external collaborators.
            This property is not modified if not specified.
            To clear the existing list, use the value of $CLEAR_VALUE_FLAG as defined in BitTitan.Runbooks.Common.
        SharingCapability
            Single string, optional.
            This sets the level of sharing available for the site collection.
            Possible values are 'Disabled', 'ExistingExternalUserSharingOnly', 'ExternalUserSharingOnly', and 'ExternalUserAndGuestSharing'.
            This property is not modified if not specified.
            Disabled - Sharing outside the organization is not allowed.
            ExistingExternalUserSharingOnly - Sharing with external users is only allowed if they already exist in the organization's directory.
            ExternalUserSharingOnly - Sharing with external users is allowed if they sign in as authenticated users.
            ExternalUserAndGuestSharing - Sharing with external users and using anonymous access links is allowed.
        SharingDomainRestrictionMode
            Single string, optional.
            This selects whether the domain 'Allow' or 'Block' list, or neither, is used to control external sharing.
            Possible values are 'None', 'AllowList' and 'BlockList'.
            This property is not modified if not specified.
            None - Neither the 'Allow' nor 'Block' list is used.
            AllowList - The 'Allow' list is used.
            BlockList - The 'Block' list is used.
    Usage option 2: Update the settings of multiple SharePoint Online site collections using a CSV
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
            The OrganizationName extended property is required - it is the portion of the domain before the '.onmicrosoft.com'
            Example: If the full domain is 'contoso.onmicrosoft.com', the OrganizationName is 'contoso'.
        SiteCollectionsCsv
            Required columns:
                Url
                    The URL of the SharePoint Online site collection
            Optional columns:
                DefaultLinkPermission
                DefaultSharingLinkType
                SharingAllowedDomains
                    One or more strings separated by a comma, with the whole string surrounded by quotes.
                    Example: "contoso.com,fabrikam.com"
                SharingBlockedDomains
                    One or more strings separated by a comma, with the whole string surrounded by quotes.
                    Example: "contoso.com,fabrikam.com"
                SharingCapability
                SharingDomainRestrictionMode
```
### OUTPUTS
```
    SharePointOnlineUpdateSiteCollectionsSharingSettingsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1
    Last updated: 16 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


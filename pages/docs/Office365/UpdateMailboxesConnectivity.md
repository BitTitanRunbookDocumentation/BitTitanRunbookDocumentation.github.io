# Office 365
## Update Mailboxes' Connectivity
### SYNOPSIS
```
    Enables/Disables protocols and interfaces for Office 365 mailboxes
```
### DESCRIPTION
```
    Enables/Disables protocols and interfaces for Office 365 mailboxes.
    The various protocols and interfaces which can be enabled/disabled are:
        - POP
        - IMAP
        - MAPI
        - OWA
        - ActiveSync
        - EWS
```
### INPUTS
```
    Usage option 1: Apply a set of enable/disable settings for protocols and interfaces to one or more user mailboxes
        Office365AdministrativeCredentials
            A single MSPComplete endpoint containing the Office 365 administrative credentials, required.
        UserMailboxes
            One or more MSPComplete end user objects, optional.
            This specifies the Office 365 users which will receive the mailbox connectivity updates.
        EnableDisablePop
            A single string, optional, valid values are 'Enable' and 'Disable' (case-insensitive).
            This specifies if POP should be enabled or disabled for the user mailbox.
        EnableDisableImap
            A single string, optional, valid values are 'Enable' and 'Disable' (case-insensitive).
            This specifies if IMAP should be enabled or disabled for the user mailbox.
        EnableDisableMapi
            A single string, optional, valid values are 'Enable' and 'Disable' (case-insensitive).
            This specifies if MAPI should be enabled or disabled for the user mailbox.
        EnableDisableOwa
            A single string, optional, valid values are 'Enable' and 'Disable' (case-insensitive).
            This specifies if OWA should be enabled or disabled for the user mailbox.
        EnableDisableActiveSync
            A single string, optional, valid values are 'Enable' and 'Disable' (case-insensitive).
            This specifies if ActiveSync should be enabled or disabled for the user mailbox.
        EnableDisableEws
            A single string, optional, valid values are 'Enable' and 'Disable' (case-insensitive).
            This specifies if EWS should be enabled or disabled for the user mailbox.
    Usage option 2: Enable/disable protocols and interfaces for mailboxes
        MailboxesCsv
            A CSV string containing information about the mailboxes which will receive connectivity
            updates.
            Required columns:
                Identity
                    This specifies the mailbox which will be updated.
                    Possible mailbox identities are:
                        - Name
                        - Display name
                        - Alias
                        - Distinguished name (DN)
                        - Canonical DN
                        - <domain name>\<account name>
                        - Email address
                        - GUID
                        - LegacyExchangeDN
                        - SamAccountName
                        - User ID or user principal name (UPN)
                MailboxProtocolOrInterface
                    This specifies the name of the mailbox protocol or interface which will be enabled
                    or disabled.
                    Possible values are (case-insensitive):
                        - POP
                        - IMAP
                        - MAPI
                        - OWA
                        - ActiveSync
                        - EWS
                EnableOrDisable
                    This specifies whether the mailbox protocol or interface is to be disabled for
                    the mailbox.
```
### OUTPUTS
```
    Office365UpdateMailboxesConnectivityCsv
        A CSV string containing information about the mailboxes which were updated, as well as an
        additional column 'UpdatedMailboxConnectivity' to indicate if the update was successful.
    Office365UpdateMailboxesConnectivityErrorMessages
        A string containing the error messages which were generated over the course of the task.
```
### NOTES
```
    Version: 1.0.0
    Last updated: 8 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


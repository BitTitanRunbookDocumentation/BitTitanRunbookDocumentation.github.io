# Exchange
## Update Security Settings
### SYNOPSIS
```
    Updates the Exchange Security-related settings
```
### DESCRIPTION
```
    Updates the Exchange Security-related settings.
    The settings which can be updated are:
        - Junk email configuration is enabled/disabled for all mailboxes
        - Data Loss Prevention policies to enable/disable
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    MailboxSafeSenderLists
        A single boolean value, optional.
        If specified to be true, the junk email configuration will be enabled for all mailboxes.
        If specified to be false, the junk email configuration will be disabled for all mailboxes.
    DlpPoliciesToEnableNames
        One or more strings separated by a newline, optional.
        This specifies the names of the Data Loss Prevention policies to enable.
    DlpPoliciesToDisableNames
        One or more strings separated by a newline, optional.
        This specifies the names of the Data Loss Prevention policies to disable.
```
### OUTPUTS
```
    None
```
### NOTES
```
    Version: 1.0.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


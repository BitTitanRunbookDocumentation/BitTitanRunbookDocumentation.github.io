# Office 365
## Enable/Disable Litigation Hold On Mailboxes
### SYNOPSIS
```
    Enables or disables litigation hold on Office 365 mailboxes
```
### DESCRIPTION
```
    Enables or disables litigation hold on Office 365 mailboxes, as well as setting the period that the litigation hold will be in effect
```
### INPUTS
```
    Usage option 1: Enable or disable litigation hold on one or more mailboxes
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        Users
            One or more MSPComplete end user objects, required.
        EnableOrDisableLitigationHold
            A single string, required.
            Valid values are 'enable' and 'disable' (case-insensitive).
        LitigationHoldDuration
            A single string, optional.
            This it the number of days the mailbox will be held in litigation hold. 
            Valid values are whole numbers greater than 0. 
            If no value is provided, this will set the mailbox on litigation hold indefinitely.
    Usage option 2: Enable or disable litigation hold on one or more mailboxes via CSV
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        LitigationHoldCsv
            Required columns:
                UserEmailAddress
                    The email address of the user.
                EnableOrDisableLitigationHold
                    Valid values are 'enable' and 'disable' (case-insensitive).
                LitigationHoldDuration
                    This it the number of days the mailbox will be held in litigation hold. 
                    Valid values are whole numbers greater than 0. 
                    If no value is provided, this will set the mailbox on litigation hold indefinitely.
```
### OUTPUTS
```
    Office365EnableDisableLitigationHoldOnMailboxesCsv
        A CSV containing all the user mailboxes which were processed by this task, as well as an additional
        column 'LitigationHoldUpdated' to indicate if the update of litigation hold is successful.
    Office365EnableDisableLitigationHoldOnMailboxesErrorMessages
         A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0.0
    Last updated: 13 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


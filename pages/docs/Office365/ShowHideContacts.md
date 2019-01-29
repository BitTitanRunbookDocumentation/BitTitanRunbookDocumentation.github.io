# Office 365
## Show / Hide Contacts on Address Lists
### SYNOPSIS
```
    Show / Hide Office 365 Contacts on Address Lists
```
### DESCRIPTION
```
    This sets the visibility of contacts on address lists, including the Global Address List (GAL).
```
### INPUTS
```
    Usage option 1: Show or hide 1 contact
        Identity
            A string value that uniquely identifies the contact, e.g. contact name or email address, required
            Example: johndoe@domain.com
        ShowOrHide
            A string value that specifies whether to show or hide the contact, case insensitive, required
            Example: Hide
    Usage option 2: Show or hide multiple contacts, using the inputs from a CSV file
        ContactsCsv
            Required Columns:
                Identity
                    A string value that uniquely identifies the contact, e.g. contact name or email address, required
                    Example: johndoe@domain.com
                ShowOrHide
                    A string value that specifies whether to show or hide the contact, case insensitive, required
                    Example: Hide
```
### OUTPUTS
```
    Office365ShowHideContactsCsv
        A CSV containing information about the contacts that were shown or hidden.
        A column 'ContactUpdated' is added to indicate if the contact update was successful.
    Office365ShowHideContactsAllErrorMessages
        A string containing all the error messages generated over the course of this task.
```
### NOTES
```
    Version: 1.1
    Last updated: 28 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


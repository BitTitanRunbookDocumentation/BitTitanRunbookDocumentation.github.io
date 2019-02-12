# Office 365
## Create Contacts
### SYNOPSIS
```
    Create Office 365 contacts
```
### DESCRIPTION
```
    This task library component creates a contact with a name and external email address.
    It creates a list of contacts from the inputs in a CSV file.
```
### INPUTS
```
    Usage option 1: Create a contact
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        ContactName
            A string representing the name of the contact, required.
            Example: John Doe
        ContactExternalEmailAddress
            A string representing the external email address of the contact, required.
            Example: johndoe@domain.com
    Usage option 2: Create a group of contacts, using the inputs in a CSV file
        ContactsCsv
            ContactName
                A string representing the name of the contact, required.
                Example: John Doe
            ContactExternalEmailAddress
                A string representing the external email address of the contact, required.
                Example: johndoe@domain.com
```
### OUTPUTS
```
    AllErrorMessages
        A string containing all the error messages generated over the course of this task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 31 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


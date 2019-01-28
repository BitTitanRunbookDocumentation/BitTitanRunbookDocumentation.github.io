# Office 365
## Update Contacts
### SYNOPSIS
```
    Update Office 365 contacts
```
### DESCRIPTION
```
    Update Office 365 contact settings using the Set-Contact cmdlet.
    This sets the values like the contact's company name, office phone number and mobile phone number, among other settings.
```
### INPUTS
```
    Usage option 1: Set the settings for 1 contact
        ContactName
            A string representing the name of the contact, required if ContactExternalEmailAddress is not provided
            Example: John Doe
        ContactExternalEmailAddress
            A string representing the external email address of the contact, required if ContactName is not provided
            Example: johndoe@domain.com
        FirstName
            A string representing the first name of the contact, optional
            Example: John
        LastName
            A string representing the last name of the contact, optional
            Example: Doe
        Company
            A string representing the company of the contact, optional
            Example: Domain Inc
        Phone
            A string representing the office phone number of the contact, optional
            Example: (425) 111 2222
        MobilePhone
            A string representing the mobile phone number of the contact, optional
            Example: (425) 555 6666
        Title
            A string representing the title of the contact, optional
            Example: Miss
        WebPage
            A string representing the web page of the contact, optional
            Example: https://domain.com
        Fax
            A string representing the fax number of the contact, optional
            Example: (425) 555 7777
        StreetAddress
            A string representing the street address of the contact, optional
            Example: 1 Main Street
        City
            A string representing the city of the contact, optional
            Example: Bellevue
        StateOrProvince
            A string representing the state or province of the contact, optional
            Example: Washington
        PostalCode
            A string representing the postal code of the contact, optional
            Example: 98005
        CountryOrRegion
            A 2-letter ISO-3166 code representing the country or region of the contact, optional
            Example: US
    Usage option 2: Set the settings for multiple contacts, using the inputs from a CSV file
        ContactsCsv
            Required Columns:
                Identity
                    A string representing either the name or external email address of the contact
                    Example: John Doe
                    Example: johndoe@domain.com
            Optional Columns:
                FirstName
                    A string representing the first name of the contact, optional
                    Example: John
                LastName
                    A string representing the last name of the contact, optional
                    Example: Doe
                Company
                    A string representing the company of the contact, optional
                    Example: Domain Inc
                Phone
                    A string representing the office phone number of the contact, optional
                    Example: (425) 111 2222
                MobilePhone
                    A string representing the mobile phone number of the contact, optional
                    Example: (425) 555 6666
                Title
                    A string representing the title of the contact, optional
                    Example: Miss
                WebPage
                    A string representing the web page of the contact, optional
                    Example: https://domain.com
                Fax
                    A string representing the fax number of the contact, optional
                    Example: (425) 555 7777
                StreetAddress
                    A string representing the street address of the contact, optional
                    Example: 1 Main Street
                City
                    A string representing the city of the contact, optional
                    Example: Bellevue
                StateOrProvince
                    A string representing the state or province of the contact, optional
                    Example: Washington
                PostalCode
                    A string representing the postal code of the contact, optional
                    Example: 98005
                CountryOrRegion
                    A 2-letter ISO-3166 code representing the country or region of the contact, optional
                    Example: US
```
### OUTPUTS
```
    Office365UpdateContactsCsv
        A CSV containing information about the contacts that were updated.
        A column 'ContactUpdated' is added to indicate if the contact update was successful.
    Office365UpdateContactsAllErrorMessages
        A string containing all the error messages generated over the course of this task.
```
### NOTES
```
    Version: 1.1
    Last updated: 24 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


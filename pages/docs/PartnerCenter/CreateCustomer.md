# Partner Center
## Create Customer v2
### SYNOPSIS
```
    Creates a Partner Center Customer
```
### DESCRIPTION
```
    Creates a Partner Center Customer
```
### INPUTS
```
    PartnerCenterAdministrativeCredentials
        A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
    Domain
        A single string, required.
        The domain for the new customer.
    CompanyName
        A single string, required.
        The company name of the new customer.
    ContactFirstName
        A single string, required.
        The first name of the contact person for the new customer.
    ContactFirstName
        A single string, required.
        The last name of the contact person for the new customer.
    ContactEmailAddress
        A single string, required.
        The email address of the contact person for the new customer.
    ContactPhoneNumber
        A single string, required.
        The phone number of the contact person for the new customer.
    AddressLine1
        A single string, required.
        The first line of the address of the new customer.
    AddressLine2
        A single string, optional.
        The second line of the address of the new customer.
    City
        A single string, required.
        The city of the address of the new customer.
    State
        A single string, required.
        The state of the address of the new customer.
        This should be the abbreviation of the state - for example, Ohio should be entered as 'OH'.
    PostalCode
        A single string, required.
        The postal code of the address of the new customer.
    Country
        A single string, required.
        The country of the address of the new customer.
        This should be the abbreviation of the country - for example, the United States should be entered as 'US'.
    Language
        A single string, required.
        The language of the new customer.
        This should be the abbreviation of the language - for example, English should be entered as 'en'.
    Culture
        A single string, required.
        The culture of the new customer.
        This should be the abbreviation of the culture - for example, English for the United States should be entered as 'en-US'.
```
### OUTPUTS
```
    None
```
### NOTES
```
    Version: 2.0.2
    Last updated: 15 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


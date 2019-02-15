# Office 365
## Retrieve User Information
### SYNOPSIS
```
    Retrieves Office 365 user information as a CSV string
```
### DESCRIPTION
```
    Retrieves Office 365 user information as a CSV string.
    The information retrieved includes:
        - First name
        - Last name
        - Display name
        - Address
        - City
        - State or province
        - Postal or zip code
        - Country or region
        - Mobile phone number
        - Company name
        - Department
        - Job title
        - License
        - Usage location
        - Primary email address
        - User principal name
        - Administrator role
        - Multi-factor authentication status
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    Users
        One or more MSPComplete end user objects, optional.
        If provided, user information will only be retrieved from Office 365 for these users.
        If not provided, user information will be retrieved from Office 365 for all users.
```
### OUTPUTS
```
    UserInformationCsv
        A CSV string containing the user information retrieved.
```
### NOTES
```
    Version: 1.1.2
    Last updated: 15 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


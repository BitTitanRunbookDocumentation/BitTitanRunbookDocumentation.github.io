# Office 365
## Create Users
### SYNOPSIS
```
    Creates Office 365 Users
```
### DESCRIPTION
```
    Creates an Office 365 user or multiple users via a CSV string
```
### INPUTS
```
    Usage option 1: Create one Office 365 user from a list of properties
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required
        FirstName
            String, Conditionally optional. Either FirstName, LastName or DisplayName must be supplied
            First name of the new user
        LastName
            String, Conditionally optional. Either FirstName, LastName or DisplayName must be supplied
            Last name of the new user
        DisplayName
            String, Conditionally optional. Either FirstName, LastName or DisplayName must be supplied
            Display name of the new user
        UserPrincipalName
            String, required
            User principal name of new user
        MobilePhoneNumber
            String, optional
            Mobile phone number of new user
        TelephoneNumber
            String, optional
            Telephone number of new user
        AddressLine1
            String, optional
            Address line 1 of new user
        City
            String, optional
            City of new user
        StateOrProvince
            String, optional
            State or province of new user
        PostalOrZipCode
            String, optional
            Postal or zip code of new user
        CountryOrRegion
            String, optional
            Country or region of new user
        Department
            String, optional
            Department of new user
        JobTitle
            String, optional
            Job title of new user
        Password
            String, optional
            Password for user's account. If a Password is not provided, one is randomly generated
        ForcePasswordChangeOnNextLogin
            Boolean, optional
            True to force user to change password on next login. False otherwise. Default is set to true
        UsageLocation
            String, optional
            Usage location code for user's account. Note, this is required to be set if assigning licenses
    Usage option 2: Create Office 365 users from a csv string
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required
        UsersInformationCsv
            Required columns:
                UserPrincipalName
                    String, required
                    User principal name of new user
            Optional columns:
                FirstName
                    String, Conditionally optional. Either FirstName, LastName or DisplayName must be supplied
                    First name of the new user
                LastName
                    String, Conditionally optional. Either FirstName, LastName or DisplayName must be supplied
                    Last name of the new user
                DisplayName
                    String, Conditionally optional. Either FirstName, LastName or DisplayName must be supplied
                    Display name of the new user
                MobilePhoneNumber
                    String, optional
                    Mobile phone number of new user
                TelephoneNumber
                    String, optional
                    Telephone number of new user
                AddressLine1
                    String, optional
                    Address line 1 of new user
                City
                    String, optional
                    City of new user
                StateOrProvince
                    String, optional
                    State or province of new user
                PostalOrZipCode
                    String, optional
                    Postal or zip code of new user
                CountryOrRegion
                    String, optional
                    Country or region of new user
                Department
                    String, optional
                    Department of new user
                JobTitle
                    String, optional
                    Job title of new user
                Password
                    String, optional
                    Password for user's account. If a Password is not provided, one is randomly generated
                ForcePasswordChangeOnNextLogin
                    Boolean, optional
                    True to force user to change password on next login. False otherwise. Default is set to true
                UsageLocation
                    String, optional
                    Usage location code for user's account. Note, this is required to be set if assigning licenses
```
### OUTPUTS
```
    Password
        The generated password when running the task for a single user
    Office365CreateUsersCsv
        A CSV string containing the information about which users were successfully created
        via an additional column 'NewlyCreated'.
        If the user already exists it will be indicated by a value in the column 'PreviouslyPresent'
    Office365CreateUsersErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1.1
    Last updated: 12 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


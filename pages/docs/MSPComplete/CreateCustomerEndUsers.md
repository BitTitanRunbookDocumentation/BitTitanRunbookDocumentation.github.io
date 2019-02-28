# MSPComplete
## Create Users
### SYNOPSIS
```
    Creates MSPComplete customer end users
```
### DESCRIPTION
```
    Creates MSPComplete customer end users.
    The end users will be created in the customer in the current MSPComplete context.
```
### INPUTS
```
    Usage option 1: Create an end user in a MSPComplete customer
        FirstName
            A single string, required.
            This is the first name of the end user to be created.
        LastName
            A single string, required.
            This is the last name of the end user to be created.
        PrimaryEmailAddress
            A single string, required.
            This is the primary email address of the end user to be created.
        UserPrincipalName
            A single string, optional.
            This is the user principal name of the end user to be created.
            It does not have to be the same value as the PrimaryEmailAddress.
    Usage option 2: Create end users in MSPComplete customers
        EndUsersCsv
            A CSV string containing information about the users to be created.
            Required columns:
                FirstName
                    A single string.
                    This is the first name of the end user to be created.
                LastName
                    A single string.
                    This is the last name of the end user to be created.
                PrimaryEmailAddress
                    A single string.
                    This is the primary email address of the end user to be created.
            Optional columns:
                UserPrincipalName
                    A single string, optional.
                    This is the user principal name of the end user to be created.
                    It does not have to be the same value as the PrimaryEmailAddress.
```
### OUTPUTS
```
    MSPCompleteCreateCustomerEndUsersCsv
        A CSV string containing information about the end users which were created, as well as an
        additional column 'EndUserCreated' to indicate if the end user was successfully created.
    MSPCompleteCreateCustomerEndUsersErrorMessages
        A string containing all of the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 2.0.0
    Date: 19 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


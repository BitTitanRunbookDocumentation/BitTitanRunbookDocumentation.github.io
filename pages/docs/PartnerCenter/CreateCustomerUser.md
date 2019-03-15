# Partner Center
## Create User(s)
### SYNOPSIS
```
    Creates new users in one or more Partner Center customers
```
### DESCRIPTION
```
    Creates new users in one or more Partner Center customers
```
### INPUTS
```
    Usage option 1: Create a new user
        PartnerCenterAdministrativeCredentials
            A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
        UserPrincipalName
            A single string, required.
            This is the user principal name of the new user.
        Password
            A single string, required.
            This is the password of the new user.
        FirstName
            A single string, optional.
            This is the first name of the new user.
        LastName
            A single string, optional.
            This if the last name of the new user.
        UsageLocation
            A single string, optional.
            This is the usage location of the new user.
            This property needs to be set in the user in order to assign licenses to that user.
        ForceChangePassword
            A single boolean variable, optional.
            If true, the user will be forced to change their password upon first logging in.
    Usage option 2: Create new users using a CSV string
        PartnerCenterAdministrativeCredentials
            A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
        UsersToCreateCsv
            A CSV string containing the information of the users to create.
            Required columns:
                UserPrincipalName
                    A single string.
                    This is the user principal name of the new user.
                Password
                    A single string.
                    This is the password of the new user.
            Optional columns:
                FirstName
                    A single string.
                    This is the first name of the new user.
                LastName
                    A single string.
                    This if the last name of the new user.
                UsageLocation
                    A single string.
                    This is the usage location of the new user.
                    This property needs to be set in the user in order to assign licenses to that user.
                ForceChangePassword
                    A single boolean variable.
                    If true, the user will be forced to change their password upon first logging in.
```
### OUTPUTS
```
    UpdatedUsersToCreateCsv
        A CSV string containing the information about the users, as well as an additional column 'CreatedUser' to indicate if the user was created.
    AllErrorMessages
        A string containing the error messages which were generated over the course of the task.
```
### NOTES
```
    Version: 1.2.3
    Last updated: 15 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


# Partner Center
## Add Role To Customer User
### SYNOPSIS
```
    Adds roles to users within one or more Partner Center customers
```
### DESCRIPTION
```
    Adds roles to users within one or more Partner Center customers
```
### INPUTS
```
    Usage option 1: Add a role to a user
        PartnerCenterAdministrativeCredentials
            A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
        User
            A MSPComplete end user object, required.
            This is the user which will be receiving the role.
    Usage option 2: Add roles to multiple users using a CSV string
        PartnerCenterAdministrativeCredentials
            A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
        UserRolesToAddCsv
            A CSV string containing information about the users and roles which will be added.
            Required columns:
                UserPrincipalName
                    A single string.
                    This the user principal name of the user which will be receiving the role.
                Role
                    A single string.
                    This is the role which will be added to the user.
            Optional columns:
                Domain
                    A single string. Either this or CustomerId must be provided.
                    This is the domain of the company which the user belongs to.
                CustomerId
                    A single string. Either this or Domain must be provided.
                    This is the customer ID of the company which the user belongs to.
```
### OUTPUTS
```
    UpdatedUserRolesToAddCsv
        A CSV string containing the information about the users and roles, as well as an additional column 'AddedRole' to indicate if the role was successfully added.
    AllErrorMessages
        A string containing the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1.2
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


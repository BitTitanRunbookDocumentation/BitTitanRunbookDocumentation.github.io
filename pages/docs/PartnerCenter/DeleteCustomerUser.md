# Partner Center
## Delete User(s)
### SYNOPSIS
```
    Deletes existing users in one or more Partner Center customers
```
### DESCRIPTION
```
    Deletes existing users in one or more Partner Center customers
```
### INPUTS
```
    Usage option 1: Delete a user
        PartnerCenterAdministrativeCredentials
            A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
        User
            A single MSPComplete end user object, required.
            This is the user which will be deleted from the customer.
    Usage option 2: Delete users using a CSV string
        PartnerCenterAdministrativeCredentials
            A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
        UsersToDeleteCsv
            A CSV string containing the information of the users to delete.
            Required columns:
                UserPrincipalName
                    This the user principal name of the user which will deleted.
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
    UpdatedUsersToDeleteCsv
        A CSV string containing the information about the users, as well as an additional column 'DeletedUser' to indicate if the user was deleted.
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


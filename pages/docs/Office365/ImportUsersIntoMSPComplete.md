# Office 365
## Import Users into MSPComplete
### SYNOPSIS
```
    Imports all users from an Office 365 tenant into MSPComplete
```
### DESCRIPTION
```
    Imports all users from an Office 365 tenant into MSPComplete.
    The users will be imported into the current MSPComplete customer in context.
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
    CreateUsers
        A single boolean value, optional, defaults to true.
        Selects whether a user should be created in MSPComplete if it does not exist in MSPComplete,
        but if it exists in Office 365.
    UpdateUsers
        A single boolean value, optional, defaults to true.
        Selects whether a user should be updated in MSPComplete to match the user in Office 365,
        if it exists in both MSPComplete and Office 365.
    DeleteUsers
        A single boolean value, optional, defaults to false.
        Selects whether a users should be deleted from MSPComplete if it exists in MSPComplete, but
        not in Office 365.
```
### OUTPUTS
```
    AllErrorMessages
        A string containing the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 2.0.0
    Date: 18 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


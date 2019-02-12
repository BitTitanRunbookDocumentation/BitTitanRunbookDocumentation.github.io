# Office 365
## Set Users' Passwords
### SYNOPSIS
```
    Sets the passwords of Office 365 users
```
### DESCRIPTION
```
    This sets one or more Office 365 users' passwords.
    An option can also be set to force the user to change their password upon the first login.
```
### INPUTS
```
    Usage option 1: Reset a user's password
        Office365AdministrativeCredentials
            A MSPComplete endpoint containing the Office 365 administrative credentials, required.
        User
            A single MSPComplete end user object, required.
            This user's password will be set by this task.
        Password
            A single string, required.
            This specifies the new password for the user.
            This password should meet the organization's Office 365 user password complexity requirements.
        ForceChangePassword
            A single boolean, optional, default value is true.
            This selects if the user is required to change their password upon the first login.
    Usage option 2: Reset users' passwords using a CSV
        Office365AdministrativeCredentials
            A MSPComplete endpoint containing the Office 365 administrative credentials, required.
        UsersCsv
            A CSV string containing information about the users and passwords to set, required.
            Required columns:
                PrimaryEmailAddress
                    A single string.
                    This is the primary email address of the user whose password will be set.
                Password
                    A single string.
                    This specifies the new password for the user.
                    This password should meet the organization's Office 365 user password complexity requirements.
            Optional columns:
                ForceChangePassword
                A single boolean, default value is true.
                This selects if the user is required to change their password upon the first login.
```
### OUTPUTS
```
    Office365SetUsersPasswordsCsv
        A CSV string containing information about the users and passwords that were set.
        An additional column 'SetPassword' is added to indicate if the user password was set
        successfully.
    Office365SetUsersPasswordsErrorMessages
        A string containing the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 11 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


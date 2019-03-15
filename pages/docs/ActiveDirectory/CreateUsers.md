# Active Directory
## Create Users
### SYNOPSIS
```
    Creates users in Active Directory
```
### DESCRIPTION
```
    Creates users in Active Directory.
    Several user properties can also be set for the user while creating it:
        - Display name
        - User principal name
        - Password
        - First name
        - Initials
        - Last name
        - Email address
        - Department
        - Path
        - Logon script path
        - Change password at logon
```
### INPUTS
```
    Usage option 1: Create a user in Active Directory
        DisplayName
            Single string, required.
            This is the display name for the new user.
        UserPrincipalName
            Single string, required.
            This is the user principal name for the new user.
        Password
            Single string, required.
            This is the password for the new user.
        FirstName
            Single string, optional.
            This is the first name for the new user.
        Initials
            Single string, optional.
            This is the initials or middle name for the new user.
        LastName
            Single string, optional.
            This is the last name for the new user.
        EmailAddress
            Single string, optional.
            This is the email address for the new user.
        Department
            Single string, optional.
            This is the department for the new user.
        Path
            Single string, optional.
            This is the path of the Organizational Unit or container for the new user.
        LogonScriptPath
            Single string, optional.
            This is the path to the user's logon script.
            This value can either be a local absolute path or a Universal Naming Convention (UNC) path.
        ChangePasswordAtLogon
            Single boolean, optional, default value is true.
            This indicates whether the user password must be changed on the next logon attempt.
    Usage option 2: Create users in Active Directory
        UsersCsv
            CSV string containing the information used to create the users
            Required columns:
                DisplayName
                    Single string, required.
                This is the display name for the new user.
                UserPrincipalName
                    Single string, required.
                    This is the user principal name for the new user.
                Password
                    Single string, required.
                    This is the password for the new user.
            Optional columns:
                FirstName
                    Single string, optional.
                    This is the first name for the new user.
                Initials
                    Single string, optional.
                    This is the initials or middle name for the new user.
                LastName
                    Single string, optional.
                    This is the last name for the new user.
                EmailAddress
                    Single string, optional.
                    This is the email address for the new user.
                Department
                    Single string, optional.
                    This is the department for the new user.
                Path
                    Single string, optional.
                    This is the path of the Organizational Unit or container for the new user.
                LogonScriptPath
                    Single string, optional.
                    This is the path to the user's logon script.
                    This value can either be a local absolute path or a Universal Naming Convention (UNC) path.
                ChangePasswordAtLogon
                    Single boolean, optional, default value is true.
                    This indicates whether the user password must be changed on the next logon attempt.
```
### OUTPUTS
```
    ActiveDirectoryCreateUsersCsv
        A CSV containing information about the users that were created, as well as additional columns 'UserCreated' to indicate if the user creation was successful, and 'UserObjectGuid' which is the ObjectGUID property of the created user.
    ActiveDirectoryCreateUsersErrorMessages
        A string containing all the error messages generated over the course of this task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 14 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


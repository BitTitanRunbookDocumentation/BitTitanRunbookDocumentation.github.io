# Office 365
## Enable/Disable Multi-Factor Authentication For Users
### SYNOPSIS
```
    Enables or disables multi-factor authentication for Office 365 users
```
### DESCRIPTION
```
    Enables or disables multi-factor authentication for Office 365 users.
```
### INPUTS
```
    Usage option 1: Enable or disable multi-factor authentication for a single user
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials.
        User
            Single MSPComplete user object, required
        EnableDisableMfa
            Single string, required
            Valid values are "enable" and "disable" (case-insensitive).
        RememberDevicesNotIssuedBefore
            Single string, optional
            This is a cutoff date, where any devices issued to the user before this date will
            require MFA setup.
            This input is only relevant when enabling MFA.
            If not provided, the default will be the current date, i.e. all devices issued to the
            user will require MFA setup.
            Valid date formats are "day month year", where month can be either the long or short
            month name (Dec or December), and year can either be the 2 or 4 digit year (10 or 2010,
            95 or 1995)
    Usage option 2: Enable or disable multi-factor authentication for multiple users via CSV
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials.
        UsersCsv
            Required columns:
                PrimaryEmailAddress
                EnableDisableMfa
            Optional columns:
                RememberDevicesNotIssuedBefore
```
### OUTPUTS
```
    Office365EnableDisableMultiFactorAuthenticationForUsersCsv
        A CSV string containing the information about the users for which MFA was enabled/disabled,
        as well as an additional column 'MfaUpdated' to indicate if MFA was successfully enabled or
        disabled.
    Office365EnableDisableMultiFactorAuthenticationForUsersErrorMessages
        A string containing all the errors messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 7 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


# Office 365
## Assign Licenses To Users
### SYNOPSIS
```
    Assigns licenses to one or more Office 365 users
```
### DESCRIPTION
```
    Assigns licenses to one or more Office 365 users
```
### INPUTS
```
    Usage option 1: Assign licenses to a user
        Users
            Single MSPComplete end user object, required
            If more than one object is provided, only the first one is used
        Licenses
            One or more license SKU IDs or SKU part numbers separated by a new line, optional
            If not provided, no licenses will be assigned to the user
            Example license SKU ID: reseller-account:ENTERPRISEPREMIUM
            Example SKU part number: ENTERPRISEPREMIUM
    Usage option 2: Assign a license to multiple users
        Users
            Multiple MSPComplete end user objects, required
        Licenses
            One license SKU ID or SKU part number, optional
            If more than one object is provided, only the first one is used
            If not provided, no licenses will be assigned to the user
            Example license SKU ID: reseller-account:ENTERPRISEPREMIUM
            Example SKU part number: ENTERPRISEPREMIUM
    Usage option 3: Assign licenses to multiple users using a CSV string
        UserLicensesCsv
            Required columns:
                PrimaryEmailAddress
            Optional columns:
                License
                    If not provided, no licenses will be assigned to the user
```
### OUTPUTS
```
    Office365AssignLicensesToUsersCsv
        A CSV containing all the users which were processed by this task, as well as an additional
        column 'AssignedLicenses' to indicate if the licenses were assigned successfully.
    Office365AssignLicensesToUsersErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0.0
    Last updated: 10 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


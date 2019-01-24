# Office 365
## Remove Licenses From Users
### SYNOPSIS
```
    Removes licenses from one or more Office 365 users
```
### DESCRIPTION
```
    Removes licenses from one or more Office 365 users
```
### INPUTS
```
    Single-Input Scenario
        User
            Single MSPC end user object, required
            If more than one object is provided, only the first one is used
        Licenses
            One or more license SKU IDs or SKU part numbers separated by a new line, optional
            If not provided, all licenses will be removed from the user
            Example license SKU ID: reseller-account:ENTERPRISEPREMIUM
            Example SKU part number: ENTERPRISEPREMIUM
    Multiple-Input Scenario
        UserLicensesCsv
            Required columns:
                PrimaryEmailAddress
            Optional columns:
                License
                    If not provided, all licenses will be removed from the user
```
### OUTPUTS
```
    ProcessedUserLicensesCsv
        A CSV containing all the users which were processed by this task, as well as an additional
        column 'RemovedLicenses' to indicate if the licenses were removed successfully.
    AllErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1.0
    Last updated: 3 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


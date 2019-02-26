# Office 365
## Import Groups into MSPComplete
### SYNOPSIS
```
    Imports all groups from an Office 365 tenant into MSPComplete
```
### DESCRIPTION
```
    Imports all groups from an Office 365 tenant into MSPComplete.
    The types of groups imported into MSPComplete are:
        -Distribution groups
        -Unified groups
        -Dynamic distribution groups
    The member lists for distribution groups and unified groups are also imported into MSPComplete.
    In order for the distribution group and unified group members to be imported, the members first
    have to be imported into MSPComplete as end users, using [Office 365] - Import Users into MSPComplete.
```
### INPUTS
```
    Office365Endpoint
        A MSPComplete endpoint containing the Office 365 administrative credentials, required.
    Customer
        A MSPComplete customer object, optional.
        This specifies the customer which will receive the imported groups from Office 365.
        If this is not provided, the groups will be imported into the customer in the MSPComplete
        context (i.e. the customer for which the runbook was launched).
    CreateGroups
        A single boolean value, optional, defaults to true.
        Selects whether a group should be created in MSPComplete if it does not exist in MSPComplete,
        but if it exists in Office 365.
    UpdateGroups
        A single boolean value, optional, defaults to true.
        Selects whether a group should be updated in MSPComplete to match the group in Office 365,
        if it exists in both MSPComplete and Office 365. Updating a group consists of both updating
        the group information as well as its membership.
    DeleteGroups
        A single boolean value, optional, defaults to false.
        Selects whether a group should be deleted from MSPComplete if it exists in MSPComplete, but
        not in Office 365.
```
### OUTPUTS
```
    AllErrorMessages
        A string containing all the error messages generated over the course of this task.
```
### NOTES
```
    Version: 1.3.1
    Date: 15 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


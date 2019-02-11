# Office 365
## Add/Remove Members From Distribution Groups
### SYNOPSIS
```
    Adds or removes members from Office 365 distribution groups
```
### DESCRIPTION
```
    Adds or removes members from Office 365 distribution groups.
    A member of a distribution group can either be a user, or another distribution group.
```
### INPUTS
```
    Usage option 1: Add or remove a user as a member from one or more distribution groups
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        AddOrRemoveMember
            A single string, required.
            Valid values are 'add' and 'remove'.
        DistributionGroup
            One or more MSPComplete group objects, required.
            This is the group(s) which the user will be added/removed from.
            The group objects need to have a 'PrimaryEmailAddress' extended property, which is the
            group's email address in Office 365.
        MemberUsers
            A single MSPComplete end user object, required.
            This is the user which will be added/removed from the group.
    Usage option 2: Add or remove a group as a member from one or more distribution groups
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        AddOrRemoveMember
            A single string, required.
            Valid values are 'add' and 'remove'.
        DistributionGroup
            One or more MSPComplete group objects, required.
            A single MSPComplete group object, required.
            This is the group(s) which the group will be added/removed from.
            The group objects need to have a 'PrimaryEmailAddress' extended property, which is the
            group's email address in Office 365.
        MemberGroups
            A single MSPComplete group object, required.
            This is the group which will be added/removed from the group.
            The group objects need to have a 'PrimaryEmailAddress' extended property, which is the
            group's email address in Office 365.
    Usage option 3: Add or remove one or more users as members from a distribution group
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        AddOrRemoveMember
            A single string, required.
            Valid values are 'add' and 'remove'.
        DistributionGroup
            A single MSPComplete group object, required.
            This is the group which the user will be added/removed from.
            The group object needs to have a 'PrimaryEmailAddress' extended property, which is the
            group's email address in Office 365.
        MemberUsers
            One or more MSPComplete end user objects, required.
            They are the users which will be added/removed from the group.
    Usage option 4: Add or remove one or more groups as members from a distribution group
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        AddOrRemoveMember
            A single string, required.
            Valid values are 'add' and 'remove'.
        DistributionGroup
            A single MSPComplete group object, required.
            This is the group which the group will be added/removed from.
            The group object needs to have a 'PrimaryEmailAddress' extended property, which is the
            group's email address in Office 365.
        MemberGroups
            One or more MSPComplete group objects, required.
            They are the groups which will be added/removed from the group.
            The group objects need to have a 'PrimaryEmailAddress' extended property, which is the
            group's email address in Office 365.
    Usage option 5: Add or remove users or groups as members from distribution groups via CSV
        Office365AdministrativeCredentials
            A single MSPComplete endpoint object, required.
            It contains the Office 365 administrative credentials.
        MembersCsv
            Required columns:
                DistributionGroupPrimaryEmailAddress
                    The primary email address of the distribution group
                AddOrRemoveMember
                    Valid values are 'add' and 'remove'
                MemberPrimaryEmailAddress
                    The primary email address of the member to add or remove from the distribution
                    group
```
### OUTPUTS
```
    Office365AddRemoveMembersFromDistributionGroupsCsv
        A CSV string containing information about the members which were added/removed from the
        distribution groups, as well as an additional column 'MembershipUpdated' to indicate if the
        members were successfully added/removed from the distribution groups.
    Office365AddRemoveMembersFromDistributionGroupsErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1
    Last updated: 1 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```


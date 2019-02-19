# MSPComplete
## Retrieve Groups
### SYNOPSIS
```
    Retrieves MSPComplete groups
```
### DESCRIPTION
```
    Retrieves MSPComplete groups.
    The MSPComplete groups are retrieved as MSPComplete group objects.
    The group objects are retrieved from the MSPComplete customer in the runbook context.
    The groups retrieved can be specified by:
        Group name
        Extended property name and values
```
### INPUTS
```
    Usage option 1: Retrieving groups which match one or more group names
        GroupNames
            One or more strings separated by a newline, required.
            The MSPComplete group will be selected if it matches any of these names.
    Usage option 2: Retrieving groups which have an extended property which matches one or more values
        GroupExtendedPropertyName
            A single string, required.
            This is the name of the extended property which will be used to check against the list
            of values.
        GroupExtendedPropertyValues
            One or more strings separated by a newline, required
            The MSPComplete group will be selected if its extended property with the name provided
            matches any of these values.
    Usage option 3: Retrieving groups using a CSV
        FiltersCsv
            Optional columns:
                GroupNames
                    One or more strings separated by a comma, enclosed in quotes.
                    Example: "groupName1,groupName2"
                    The MSPComplete group will be selected if it matches any of these names.
                GroupExtendedPropertyName
                    A single string.
                    If a value for this column is specified, a value for GroupExtendedPropertyValues
                    must be specified.
                    This is the name of the extended property which will be used to check against
                    the list of values.
                GroupExtendedPropertyValues
                    One or more strings separated by a comma, enclosed in quotes.
                    Example: "value1,value2"
                    If a value for this column is specified, a value for GroupExtendedPropertyName
                    must be specified.
                    The MSPComplete group will be selected if its extended property with the name
                    provided matches any of these values.
            If GroupNames, GroupExtendedPropertyName and GroupExtendedPropertyValues are all
            specified together, then the MSPComplete group will be selected only if its name matches
            the names in GroupNames AND it has an extended property with the name
            GroupExtendedPropertyName which matches one of the values in GroupExtendedPropertyValues.
```
### OUTPUTS
```
    MSPCompleteRetrievedGroups
        This contains the group objects which are retrieved by this task which match the specified
        filters.
    MSPCompleteRetrieveGroupsErrorMessages
        A string containing all the errors messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0.1
    Last updated: 7 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

